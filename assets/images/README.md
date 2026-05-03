# Adding Your Profile Photo

This directory holds images used by the GitHub Pages site.

## Steps to add your headshot

**1. Prepare your photo**
- File name: `headshot.jpg` (or `.png`)
- Recommended size: 400×400 px minimum, square crop
- File size: under 500 KB

**2. Upload the file**

Option A — via GitHub web UI:
1. Navigate to `assets/images/` in your repository on GitHub
2. Click **Add file → Upload files**
3. Upload your headshot and name it `headshot.jpg`
4. Commit directly to `main`

Option B — via command line:
```bash
cp /path/to/your/photo.jpg assets/images/headshot.jpg
git add assets/images/headshot.jpg
git commit -m "Add profile headshot"
git push
```

**3. Activate the image in index.md**

Open `index.md` and find the comment block near the top that reads:

```
<!-- ============================================================
  PROFILE PHOTO — add your headshot here
  ...
============================================================ -->
```

Delete that entire comment block and replace it with this single line:

```markdown
![Olusola B. Akanji]({{ site.baseurl }}/assets/images/headshot.jpg){: style="float: right; margin: 0 0 1.5em 1.5em; width: 150px; border-radius: 6px;"}
```

The photo will appear floated to the right of your name and summary on the rendered site.

**4. Adjust size if needed**

Change `width: 150px` in the style attribute to make the photo larger or smaller. `160px`–`200px` works well for most layouts.
