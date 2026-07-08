# Phishing Investigations

This directory contains SOC investigation reports related to phishing alerts. These cases involve analyzing suspicious emails, evaluating URLs, verifying whether payloads were delivered, and identifying indicators of compromise (IOCs) such as malicious domains or attachments.

## Current Cases

| Type | Case | Event ID | Alert Name | Summary | Report Link |
| --- | --- | --- | --- | --- | --- |
| Phishing Mail | **SOC114** | 45 | Malicious Attachment Detected | Investigated a true positive malicious attachment alert (CVE-2017-11882). | [SOC114 Report](SOC114-Malicious-Attachment-Detected.md) |
| Phishing Mail | **SOC120** | 52 | Phishing Mail Detected - Internal to Internal | Investigated an internal-to-internal phishing alert and verified it as a false positive. | [SOC120 Report](SOC120-Phishing-Mail-Detected.md) |
| Phishing Mail | **SOC140** | 82 | Phishing Mail Detected - Suspicious Task Scheduler | Investigated a blocked phishing email containing a link to a ZIP payload associated with a suspicious Task Scheduler alert. | [SOC140 Report](SOC140-Phishing-Mail-Detected.md) |
| Phishing URL | **SOC141** | 86 | Phishing URL Detected | Investigated an alert for a malicious phishing URL being allowed and successfully delivered to an endpoint. | [SOC141 Report](SOC141-Phishing-URL-Detected.md) |
| Phishing Mail | **SOC146** | 93 | Phishing Mail Detected | Investigated an email bypassing the gateway containing a malicious legacy Excel 4.0 Macro attachment. | [SOC146 Report](SOC146-Phishing-Mail-Detected.md) |
| Phishing | **SOC338** | 316 | Lumma Stealer - DLL Side-Loading via Click Fix Phishing | Investigated a true positive phishing alert involving DLL Side-Loading. | [SOC338 Report](SOC338-Lumma-Stealer.md) |
