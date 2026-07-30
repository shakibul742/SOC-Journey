# SOC140 - Phishing Mail Detected

| Field | Value |
|---------|---------|
| Alert Name | SOC140 - Phishing Mail Detected - Suspicious Task Scheduler (EventID: 82 from LetsDefend) |
| Date Investigated | 2026-06-20 |
| Event Time | Mar, 21, 2021, 12:26 PM |
| Skill Level | Easy |
| Verdict | True Positive |
| Time Spent | 20 mins |

## 1. Threat Frameworks & Impact

- **MITRE ATT&CK:**
  - T1566.002 – Phishing: Spearphishing Link
- **CVE:** N/A
- **Impact:** Medium

## 2. The "Why" (Core Evidence)

- The alert was triggered because a malicious phishing mail was detected.
- Since the action was marked as "Blocked," the malicious payload was failed delivered to the endpoint.

## 3. Key IOCs

- **Phishing URL** `https://download.cyberlearn.academy/download/download?url=https://files-ld.s3.us-east-2.amazonaws.com/72c812cf21909a48eb9cceb9e04b865d.zip`
- **Malicious Hash** `72c812cf21909a48eb9cceb9e04b865d`

## 4. Action Taken & Takeaway

- **Action:** Delete the email.

## 5. References

- **Investigation Report (LetsDefend):**
  - https://app.letsdefend.io/case-management/casedetail/shakibul742/93

- **Official MITRE ATT&CK:**
  - https://attack.mitre.org/techniques/T1566/002/

- **Write-ups Reviewed:**
  - https://medium.com/@higherdas09/letsdefend-soc140-phishing-mail-detected-event-id-82-dc88e1134d7e