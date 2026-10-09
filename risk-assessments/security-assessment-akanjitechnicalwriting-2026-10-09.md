# Security and Optimization Assessment Report
**Subject:** akanjitechnicalwriting.com
**Date:** October 9, 2026
**Prepared by:** Olusola Akanji, GRC Analyst

---

## Executive Summary

A full security and performance review of akanjitechnicalwriting.com identified one critical vulnerability, seven high-severity vulnerabilities, and four optimization gaps across dependency management, HTTP security headers, metadata, and asset hygiene. All findings were remediated in a single session. The site now has a clean dependency audit, a complete HTTP security header profile, and correct structured data on all blog posts.

---

## Scope

This assessment covered the full production stack for akanjitechnicalwriting.com:

- Static site source code (Astro 7.x, Node.js 22)
- npm dependency tree (346 packages audited)
- CloudFront distribution response header policy
- GitHub Actions CI/CD pipeline
- Built asset inventory (images, fonts, JavaScript bundles)
- HTML output (meta tags, structured data, robots directives)

---

## Findings and Remediations

### 1. Critical: Remote Code Execution in Astro Core

**Finding:** Astro version 7.2.2 contained two actively tracked vulnerabilities: remote code execution via malformed AVIF image processing (GHSA-26w7-cxv4-gfx2) and an authorization bypass from a path-segment boundary check failure (GHSA-376h-93r7-7g6f).

**Why it matters:** The AVIF RCE vulnerability creates an attack vector during the build process. Any pipeline that processes externally sourced images, including CI/CD jobs triggered by pull requests, could be exploited to execute arbitrary code in the build environment.

**Remediation:** Updated Astro from 7.2.2 to 7.3.8 via `npm audit fix`. Both CVEs are patched in 7.3.8.

---

### 2. High: Seven Additional Dependency Vulnerabilities

**Finding:** `npm audit` identified high-severity issues in seven additional packages: `sharp` (libheif and librsvg vulnerabilities in the image processing pipeline), `undici` (eleven DoS and response-splitting issues), `devalue` (serialization exploits and sparse-array CPU amplification), `source-map-js` (event-loop DoS via indexed source-map section offsets), `svgo` (incomplete script sanitization in SVG foreignObject elements), `js-yaml` (unbounded CPU use from empty merge keys), and `http-cache-semantics` (cross-user cached response disclosure).

**Why it matters:** Most of these vulnerabilities affect build-time tooling rather than the served static output. However, the `undici` issues affect HTTP request handling and the `source-map-js` DoS could destabilize the build process under adversarial input. `http-cache-semantics` is a concern if the build pipeline handles authenticated content.

**Remediation:** All seven resolved via `npm audit fix`. Zero vulnerabilities remain.

---

### 3. Medium: Incomplete HTTP Security Header Profile

**Finding:** The existing CloudFront Response Headers Policy covered HSTS, X-Frame-Options, X-Content-Type-Options, Referrer-Policy, and a Content Security Policy. Two gaps were identified:

- `Permissions-Policy` was absent, leaving browser APIs (camera, microphone, geolocation) unrestricted.
- The CSP `connect-src` directive did not include `https://api.hsforms.com`, which would silently block form submissions from the ISO 42001 Readiness Calculator's HubSpot lead capture.

**Why it matters:** A missing `Permissions-Policy` allows any third-party script loaded in the page to request access to sensitive browser APIs. The `connect-src` gap was a functional bug masquerading as a security gap: the HubSpot form would fail silently for any user whose browser enforced CSP strictly.

**Remediation:** Updated the existing CloudFront Response Headers Policy to add `Permissions-Policy` and extend `connect-src`.

**Final header profile:**

| Header | Value |
|---|---|
| `Strict-Transport-Security` | `max-age=63072000; includeSubDomains; preload` |
| `X-Frame-Options` | `DENY` |
| `X-Content-Type-Options` | `nosniff` |
| `X-XSS-Protection` | `1; mode=block` |
| `Referrer-Policy` | `strict-origin-when-cross-origin` |
| `Content-Security-Policy` | `default-src 'self'; script-src 'self'; style-src 'self' 'unsafe-inline'; img-src 'self' data: https:; connect-src 'self' https://api.hsforms.com; frame-ancestors 'none'` |
| `Permissions-Policy` | `camera=(), microphone=(), geolocation=()` |

---

### 4. Low: Incomplete Twitter/X Card Meta Tags

**Finding:** `BaseHead.astro` set `twitter:card` but omitted `twitter:title`, `twitter:description`, and `twitter:image`. Shared links on X would render without a title, description, or preview image.

**Why it matters:** Incomplete Open Graph and Twitter card metadata reduces click-through rate on shared content. For a portfolio and content marketing site, social sharing quality directly affects audience reach.

**Remediation:** Added the three missing Twitter meta tags to `BaseHead.astro`. Blog posts now also pass their `heroImage` to `BaseHead`, correcting a secondary issue where all pages defaulted to the site-level placeholder image regardless of post-specific content.

---

### 5. Low: Missing robots.txt

**Finding:** No `robots.txt` file existed in the public directory. The sitemap was correctly generated at `/sitemap-index.xml` but was not referenced by a robots directive.

**Why it matters:** Without a `robots.txt`, search crawlers have no explicit signal to follow. The absence also means the sitemap location is not surfaced to crawlers that check `robots.txt` before crawling.

**Remediation:** Created `public/robots.txt` allowing all agents and referencing the sitemap URL.

---

### 6. Low: Missing Structured Data on Blog Posts

**Finding:** No `application/ld+json` blocks existed anywhere on the site. Blog posts had no `BlogPosting` schema.

**Why it matters:** Structured data (JSON-LD) is the mechanism Google uses to generate rich results in search: article publication dates, author attribution, breadcrumbs, and enhanced previews. Without it, all 20 blog posts are treated as generic web pages with no semantic context.

**Remediation:** Added `BlogPosting` schema to `BlogPost.astro`. Each post now emits a structured data block containing headline, description, datePublished, dateModified, author (name and URL), publisher, mainEntityOfPage, and image.

---

### 7. Low: 12 MB of Unreferenced Image Assets

**Finding:** The `src/assets/` directory contained 11 files not referenced by any page: five duplicate PNG versions of images whose blog posts reference the JPG versions (each PNG averaging 1.9 MB), five Astro starter template placeholders, and one orphaned middle image. Total unreferenced weight: approximately 12 MB.

**Why it matters:** Unreferenced source assets do not affect served file size (Astro only processes referenced files) but they inflate repository size, slow clone and CI checkout times, and create confusion about which assets are canonical.

**Remediation:** Deleted all 11 files. Three additional orphaned images were retained pending potential use in planned posts.

---

## Current Security Posture

The site is a fully static deployment. There is no server-side execution surface. All dynamic behavior runs in the browser against hardcoded data. User input (the HubSpot lead form in the ISO 42001 Readiness Calculator) is transmitted directly to HubSpot's API and is not stored or processed by site infrastructure.

The primary security controls in place:

- **Dependency hygiene:** 0 known vulnerabilities across 346 packages.
- **Transport security:** HSTS enforced for 2 years with subdomains and preload.
- **Clickjacking protection:** X-Frame-Options DENY prevents the site from being embedded in iframes.
- **Content injection protection:** CSP restricts script execution to same-origin bundled files. No eval, no CDN-loaded scripts, no inline script execution.
- **XSS review:** All `innerHTML` assignments in the interactive tools inject hardcoded static data from bundled JSON. No user-controlled strings are rendered into the DOM.
- **Secrets management:** AWS credentials are stored in GitHub Secrets. No credentials, tokens, or private keys are present in source code.

---

## Residual Considerations

**GitHub Actions pinning.** The workflow uses floating `@v4` tags for `actions/checkout`, `actions/setup-node`, and `aws-actions/configure-aws-credentials`. If a malicious commit were tagged `v4` on any of these repositories, it would execute in the build environment with access to AWS credentials. Pinning to commit SHAs eliminates this vector. This is a low-probability risk for a personal project but is standard practice for production pipelines.

**Default OG image.** Pages without a hero image (tool pages, about page) still fall back to `blog-placeholder-1.jpg` as the Open Graph preview image. A branded OG default would improve social sharing quality for non-post pages.

**CSP and inline styles.** The current `style-src 'self' 'unsafe-inline'` directive permits inline styles, which Astro uses extensively for component-scoped CSS variables. Tightening this to use a nonce would require Astro SSR mode, which is not compatible with the current static deployment model.

---

*Report covers work completed October 9, 2026. All remediations applied to production.*
