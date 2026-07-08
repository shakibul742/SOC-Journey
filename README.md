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
| Web Attack | IDOR | SOC169 | 119 | Investigated an alert for a possible IDOR attack. | [Report](./SOC-Investigation-Report/Web-Attack/IDOR/SOC169-Possible-IDOR-Attack-Detected.md) |
| Web Attack | Command Injection | SOC167 | 117 | Investigated a potential command injection alert (false positive). | [Report](./SOC-Investigation-Report/Web-Attack/LS/SOC167-LS-Command-Detected.md) |
| Phishing | URL | SOC141 | 86 | Investigated an alert for a malicious phishing URL being allowed and successfully delivered to an endpoint. | [Report](./SOC-Investigation-Report/Phishing/SOC141-Phishing-URL-Detected.md) |
| Phishing | Mail | SOC146 | 93 | Investigated an email bypassing the gateway containing a malicious legacy Excel 4.0 Macro attachment. | [Report](./SOC-Investigation-Report/Phishing/SOC146-Phishing-Mail-Detected.md) |
| Phishing | Mail | SOC114 | 45 | Investigated a true positive malicious attachment alert (CVE-2017-11882). | [Report](./SOC-Investigation-Report/Phishing/SOC114-Malicious-Attachment-Detected.md) |
| Phishing | Mail | SOC120 | 52 | Investigated an internal-to-internal phishing alert and verified it as a false positive. | [Report](./SOC-Investigation-Report/Phishing/SOC120-Phishing-Mail-Detected.md) |
| Phishing | Mail | SOC140 | 82 | Investigated a blocked phishing email containing a link to a ZIP payload associated with a suspicious Task Scheduler alert. | [Report](./SOC-Investigation-Report/Phishing/SOC140-Phishing-Mail-Detected.md) |
| Phishing | Lumma Stealer | SOC338 | 316 | Investigated a true positive phishing alert involving DLL Side-Loading. | [Report](./SOC-Investigation-Report/Phishing/SOC338-Lumma-Stealer.md) |
| Brute Force | RDP | SOC176 | 234 | Investigated an alert for multiple failed RDP login attempts followed by a successful authentication, resulting in account compromise. | [Report](./SOC-Investigation-Report/Brute%20Force/SOC176-RDP-Brute-Force-Detected.md) |
| Powershell | Suspicious Execution | SOC153 | 238 | Investigated an alert for a suspicious PowerShell script execution leading to a successful C2 connection. | [Report](./SOC-Investigation-Report/Powershell/SOC153-Suspicious-Powershell-Script-Executed.md) |
| Unauthorized Access | VPN | SOC257 | 225 | Investigated an alert for a successful VPN connection from an unauthorized country following brute-force attempts. | [Report](./SOC-Investigation-Report/Unauthorized%20Access/SOC257-VPN-Connection-Detected.md) |

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