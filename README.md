# SOC Analyst Portfolio

Welcome to my cybersecurity portfolio! This repository serves as a centralized hub documenting my hands-on practice, alert triage, and incident investigations as an aspiring Security Operations Center (SOC) Analyst. Each report is intended to show the investigation process from alert review through validation, findings, and final classification.

## Focus Areas
- **Alert Triage & Investigation**: Analyzing SIEM alerts to distinguish true positives from false positives.
- **Log Analysis**: Reading through HTTP, firewall, and endpoint logs.
- **Threat Hunting Basics**: Identifying indicators of compromise (IOCs) such as malicious domains, IP addresses, and hashes.
- **Incident Response**: Detailing containment steps and remediation lessons learned.

## SOC Investigation Reports

This section contains fully documented case studies of simulated alerts I have investigated. Each report follows a structured approach mapping to the MITRE ATT&CK framework.

### Investigation Categories

- **[Web Attack Investigations](./SOC-Investigation-Report/Web-Attack/)**: Cases analyzing malicious web traffic, payload execution, and vulnerabilities (e.g., XSS, LFI, IDOR, Command Injection).
- **[Phishing Investigations](./SOC-Investigation-Report/Phishing/)**: Cases involving malicious emails, URLs, and attachments.
- **[Brute Force](./SOC-Investigation-Report/Brute%20Force/)**: Investigations into brute force attacks and account compromises.
- **[Powershell](./SOC-Investigation-Report/Powershell/)**: Analysis of suspicious PowerShell script executions.
- **[Unauthorized Access](./SOC-Investigation-Report/Unauthorized%20Access/)**: Investigations into unauthorized logins (e.g., VPN connections from unauthorized countries).

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