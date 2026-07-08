# SOC338 - Lumma Stealer - DLL Side-Loading via Click Fix Phishing

| Field | Value |
|---------|---------|
| Alert Name | SOC338 - Lumma Stealer - DLL Side-Loading via Click Fix Phishing (EventID: 316 from LetsDefend) |
| Date Investigated | 2026-07-04 |
| Event Time | Mar, 13, 2025, 09:44 AM |
| Verdict | True Positive |
| Time Spent | 25 mins |

## 1. Threat Frameworks & Impact

- **MITRE ATT&CK:**
  - T1566.001 – Phishing: Spearphishing Attachment
- **CVE:** N/A
- **Impact:** Critical

## 2. The "Why" (Core Evidence)

- The alert was triggered because a malicious Url was detected.
- The email was successfully delivered to the recipient because the email gateway allowed it.
- The phishing email opened by Dylan User.

## 3. Key IOCs

- **Phishing URL** `https://www.windows-update.site/`
- **SMTP Address** `103.80.134.63`
- **Source Address** `accounting@cmail.carleton.ca`
- **Sender Domain** `windows-update.site``

## 4. Action Taken

- Deleted the phishing email from the recipient's mailbox.
- Contained the affected user (**Dylan**) to prevent further malicious activity.