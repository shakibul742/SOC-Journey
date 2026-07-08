# Web Attack Investigations

This directory contains SOC investigation reports related to web-based attacks. These cases focus on analyzing HTTP traffic, identifying malicious payloads in URLs or body content, and determining if the attack (such as XSS, SQLi, etc.) was successful or blocked.

## Current Cases

| Type | Case | Event ID | Alert Name | Summary | Report Link |
| --- | --- | --- | --- | --- | --- |
| XSS | **SOC166** | 116 | XSS Attack Attempt | Investigated a SIEM alert for JavaScript detected in a requested URL and confirmed it as a true positive, unsuccessful XSS attempt. | [XSS Report](XSS/README.md) |
| LFI | **SOC170** | 120 | Passwd Found in Requested URL - Possible LFI Attack | Investigated a SIEM alert for a possible LFI attack involving a passwd file requested in a URL. | [SOC170 Report](LFI-RFI/SOC170-Possible-LFI-Attack.md) |
| IDOR | **SOC169** | 119 | Possible IDOR Attack Detected | Investigated an alert for a possible IDOR attack. | [SOC169 Report](IDOR/SOC169-Possible-IDOR-Attack-Detected.md) |
| Command Injection | **SOC167** | 117 | LS Command Detected in Requested URL | Investigated a potential command injection alert (false positive). | [SOC167 Report](LS/SOC167-LS-Command-Detected.md) |
