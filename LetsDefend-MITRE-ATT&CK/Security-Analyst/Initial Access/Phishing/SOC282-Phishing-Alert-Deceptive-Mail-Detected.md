##  SOC282 - Phishing Alert - Deceptive Mail Detected

| Field | Value |
|---------|---------|
| Alert Name | SOC282 - Phishing Alert - Deceptive Mail Detected (EventID: 257 from LetsDefend) |
| Date Investigated | 2026-07-31 |
| Event Time | May, 13, 2024, 09:22 AM |
| Skill Level | Medium |
| Verdict | True Positive |
| Time Spent | 32 mins |


## Analyst Note

On May, 13, 2024 at 09:22 AM the SOC282 - Phishing Alert - Deceptive Mail Detected alert was triggered. After investigation, the email contain malicious file url. Log clearly shows that the email was delivered and the mail was opened. So the alert was true positive.


## Artifacts

- **SMTP Address** `103.80.134.63`
- **Malicious File Url** `https://download.cyberlearn.academy/download/download?url=https://files-ld.s3.us-east-2.amazonaws.com/59cbd215-76ea-434d-93ca-4d6aec3bac98-free-coffee.zip`
- **Source Address** `free@coffeeshooop.com`
- **Process** `Coffee.exe`


## Threat Frameworks & Impact

- **MITRE ATT&CK:**
  - T1566.001 - Spearphishing Attachment
- **CVE:** N/A
- **SEVERITY:** Medium


## Action Taken

- Deleted the phishing email from the recipient's mailbox.
- Contained the affected user (**Felix**) to prevent further malicious activity.


## References

- **Investigation Report (LetsDefend):**
  - https://app.letsdefend.io/case-management/casedetail/shakibul742/257

- **Official MITRE ATT&CK:**
  - https://attack.mitre.org/techniques/T1566/001/

- **Write-ups Reviewed After Investigation:**
  - https://medium.com/@topcyberdawg/letsdefend-soc-walkthrough-soc282-phishing-alert-deceptive-mail-detected-0360c11b162c