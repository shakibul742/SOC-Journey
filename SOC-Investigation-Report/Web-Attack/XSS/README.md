# SOC Investigation: XSS Attack Attempt

## Overview
This project documents a SOC investigation involving a suspected Cross-Site Scripting (XSS) attack detected through a SIEM alert. The analysis focuses on log analysis, HTTP traffic inspection, and attack validation.

## Alert Details
- **Case**: SOC166
- **Event ID**: 116
- **Rule**: JavaScript Code Detected in Requested URL
- **Severity**: Medium
- **Category**: Web Attack (XSS)

## Key Findings
- An external IP attempted multiple XSS payload injections (script, SVG, event-based).
- Traffic direction: Internet to Internal Network.
- The server responded with HTTP 302 and no content for malicious requests.
- No evidence of payload execution or compromise was found.

## Conclusion
The alert was validated as a **True Positive**, representing an **unsuccessful XSS attack attempt**. This case highlights the importance of distinguishing between attack attempts and successful exploitation using HTTP response analysis.

## Report
[View PDF Report](Event_ID_116_XSS_Attack_Investigation_Report.pdf)
