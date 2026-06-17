# Web Attack Investigations

This directory contains SOC investigation reports related to web-based attacks. These cases focus on analyzing HTTP traffic, identifying malicious payloads in URLs or body content, and determining if the attack (such as XSS, SQLi, etc.) was successful or blocked.

## Current Cases

| Type | Case | Event ID | Alert Name | Summary | Report Link |
| --- | --- | --- | --- | --- | --- |
| XSS | N/A | 116 | XSS Attack Attempt | Investigated a SIEM alert for JavaScript detected in a requested URL and confirmed it as a true positive, unsuccessful XSS attempt. | [XSS Report](XSS/README.md) |
| LFI | **SOC170** | 120 | Passwd Found in Requested URL - Possible LFI Attack | Investigated a SIEM alert for a possible LFI attack involving a passwd file requested in a URL. | [SOC170 Report](LFI-RFI/SOC170%20-Possible-LFI-Attack.md) |
