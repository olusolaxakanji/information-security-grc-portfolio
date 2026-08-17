# Evidence

This directory holds the evidence records produced by running controls in the Emyzer Technology GRC programme.

## Directory Structure

```
evidence/
├── README.md
├── 2025/
│   ├── ET-CTRL-001/     # One folder per control ID, per year
│   ├── ET-CTRL-002/
│   ├── ET-CTRL-003/
│   ├── ET-CTRL-004/
│   ├── ET-CTRL-005/
│   ├── ET-CTRL-006/
│   ├── ET-CTRL-007/
│   └── ET-CTRL-008/
└── 2024/
    └── ...
```

Each control folder contains evidence files named with the test date and a short description:

```
2025/ET-CTRL-001/
├── 2025-09-30_access-review-q3.md
└── 2025-06-30_access-review-q2.md
```

## File Naming

```
YYYY-MM-DD_short-description.md
```

## What Belongs Here

- Test result summaries: pass/fail status, exceptions noted, remediation taken
- Access review certification records
- Training completion reports
- Tabletop exercise after-action reports
- Vendor risk assessment outputs

## Related

| Document | Description |
|---|---|
| [Controls Library](../controls/README.md) | The controls that produce these evidence records |
| [ServiceNow Evidence](../servicenow-evidence/README.md) | Platform exports showing policy governance in ServiceNow GRC |
