# SOC146 - Phishing Mail Detected

| Field | Value |
|---------|---------|
| Alert Name | SOC146 - Phishing Mail Detected - Excel 4.0 Macros (EventID: 93 from LetsDefend) |
| Date Investigated | 2026-06-15 |
| Event Time | 2021-06-13 02:13 PM |
| Verdict | True Positive |
| Time Spent | 25 mins |

## 1. Threat Frameworks & Impact

- **MITRE ATT&CK:** T1566.001 - Spearphishing Attachment \| T1059.005 - Visual Basic / Legacy Office Scripting
- **CVE:** N/A (Abuse of legitimate legacy Excel 4.0 / XLM Macro feature)
- **Impact:** High \| Integrity & Confidentiality

## 2. The "Why" (Core Evidence)

- Alert triggered on an email bypassing the gateway (Device Action: Allowed) containing a documented Excel 4.0 Macro, a legacy feature heavily abused by malware families like Emotet, Qakbot, and Trickbot.
- Because the action was "Allowed," the malicious payload successfully landed in the user's inbox (`lars@letsdefend.io`).

## 3. Key IOCs

- **Attachment Link:**  
  `https://download.cyberlearn.academy/download/download?url=https://files-ld.s3.us-east-2.amazonaws.com/11f44531fb088d31307d87b01e8eabff.zip.zip`

## 4. Action Taken & Takeaway

- **Action:** Delete the email.
- **Lesson:** Excel 4.0 (XLM) macros are harder for standard antiviruses to analyze than modern VBA macros. When the device action is "Allowed," the investigation must immediately pivot from the email gateway to the endpoint logs to verify user interaction.
