# SOC114 - Malicious Attachment Detected

| Field | Value |
|---------|---------|
| Alert Name | SOC114 - Malicious Attachment Detected - Phishing Alert (EventID: 45 from LetsDefend) |
| Date Investigated | 2026-07-01 |
| Event Time | Jan, 31, 2021, 03:48 PM |
| Verdict | True Positive |
| Time Spent | 47 mins |

## 1. Threat Frameworks & Impact

- **MITRE ATT&CK:**
  - T1566.001 – Phishing: Spearphishing Attachment
- **CVE:** cve-2017-11882
- **Impact:** High

## 2. The "Why" (Core Evidence)

- The alert was triggered because a malicious attachment was detected.
- The email was successfully delivered to the recipient because the email gateway allowed it.
- The phishing email contained a malicious Microsoft Excel attachment.
- Log analysis confirmed communication with a malicious C2 server, indicating that the attachment was executed successfully.

## 3. Key IOCs

- **Phishing URL** `https://download.cyberlearn.academy/download/download?url=https://files-ld.s3.us-east-2.amazonaws.com/c9ad9506bcccfaa987ff9fc11b91698d.zip`
- **Malicious Hash** `c9ad9506bcccfaa987ff9fc11b91698d`
- **SMTP Address** `49.234.43.39`
- **Source Address** `accounting@cmail.carleton.ca`
- **Sender Domain** `cmail.carleton.ca`
- **Malicious IP** `5.135.143.133`
- **Malicious Domain** `andaluciabeach.net`
- **Downloaded Payload** `network.exe`

## 4. Action Taken

- Deleted the phishing email from the recipient's mailbox.
- Contained the affected user (**richard**) to prevent further malicious activity.

## References

- **My Letsdefend Report:** https://app.letsdefend.io/case-management/casedetail/shakibul742/45 

- **Official MITRE ATT&CK:** https://attack.mitre.org/techniques/T1566/001/

- **Write-ups Reviewed:** https://leyla-aliyeva.medium.com/soc114-malicious-attachment-detected-phishing-alert-investigation-7b4fb0283ce2