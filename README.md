# SOC Analyst Portfolio

Welcome to my cybersecurity portfolio! This repository serves as a centralized hub documenting my hands-on practice, alert triage, and incident investigations as an aspiring Security Operations Center (SOC) Analyst. Each report is intended to show the investigation process from alert review through validation, findings, and final classification.

## Focus Areas
- **Alert Triage & Investigation**: Analyzing SIEM alerts to distinguish true positives from false positives.
- **Log Analysis**: Reading through HTTP, firewall, and endpoint logs.
- **Threat Hunting Basics**: Identifying indicators of compromise (IOCs) such as malicious domains, IP addresses, and hashes.
- **Incident Response**: Detailing containment steps and remediation lessons learned.

## SOC Investigation Reports

This section contains fully documented case studies of simulated alerts I have investigated. Each report follows a structured approach mapping to the MITRE ATT&CK framework.

### Current Reports

| Category | Type | Case | Event ID | Summary | Links |
| --- | --- | --- | --- | --- | --- |
| Web Attack | XSS | SOC166 | 116 | Investigated a SIEM alert for JavaScript detected in a requested URL and confirmed it as a true positive, unsuccessful XSS attempt. | [README](./SOC-Investigation-Report/Web-Attack/XSS/README.md) \| [PDF Report](./SOC-Investigation-Report/Web-Attack/XSS/Event_ID_116_XSS_Attack_Investigation_Report.pdf) |
| Web Attack | LFI | SOC170 | 120 | Investigated a SIEM alert for a possible LFI attack involving a passwd file requested in a URL. | [Report](./SOC-Investigation-Report/Web-Attack/LFI-RFI/SOC170-Possible-LFI-Attack.md) |
| Phishing | URL | SOC141 | 86 | Investigated an alert for a malicious phishing URL being allowed and successfully delivered to an endpoint. | [Report](./SOC-Investigation-Report/Phishing/SOC141-Phishing-URL-Detected.md) |
| Phishing | Mail | SOC146 | 93 | Investigated an email bypassing the gateway containing a malicious legacy Excel 4.0 Macro attachment. | [Report](./SOC-Investigation-Report/Phishing/SOC146-Phishing-Mail-Detected.md) |

### Investigation Method
- Review alert metadata and severity
- Analyze related logs and web requests
- Validate whether the attack was successful or blocked
- Record findings, conclusion, and supporting report material

## Learning Platforms & Tools
- **LetsDefend**: Primary platform for hands-on SOC Analyst path and incident simulations.
- **Tools Used**: SIEM, VirusTotal, Any.Run, Exiftool, Volatility, URLhaus, etc.

## Current Level
- **Beginner / Entry-level SOC Analyst** (Actively Learning and Practicing)

## Disclaimer
All activities, investigations, and logs documented in this repository are strictly based on safe labs, simulations, and training environments. No actual corporate or personal data is involved.