# SOC Investigation Reports

This folder contains documented SOC investigation cases completed in lab and training environments. Each report is intended to show the investigation process from alert review through validation, findings, and final classification.

## Purpose
- Document incident investigations in a structured format
- Practice alert triage, log analysis, and attack validation
- Build a portfolio of SOC analyst case reports

## Investigation Areas
- Web Attacks
- SIEM Alert Analysis
- HTTP Traffic Review
- Incident Classification

## Current Reports

| Category | Case | Summary | Links |
| --- | --- | --- | --- |
| Web Attack | XSS Attack Attempt | Investigated a SIEM alert for JavaScript detected in a requested URL and confirmed it as a true positive, unsuccessful XSS attempt. | [README](Web-Attack/XSS/README.md) \| [PDF Report](Web-Attack/XSS/Event_ID_116_XSS_Attack_Investigation_Report.pdf) |

## Folder Structure

```text
SOC-Investigation-Report/
├── README.md
└── Web-Attack/
    └── XSS/
        ├── README.md
        └── Event_ID_116_XSS_Attack_Investigation_Report.pdf
```

## Method Used
- Review alert metadata and severity
- Analyze related logs and web requests
- Validate whether the attack was successful or blocked
- Record findings, conclusion, and supporting report material

## Note
All investigations in this folder are based on lab exercises, simulated scenarios, or training platforms such as LetsDefend.
