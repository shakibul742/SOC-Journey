##  SOC251 - Quishing Detected (QR Code Phishing)

| Field | Value |
|---------|---------|
| Alert Name | SOC251 - Quishing Detected (QR Code Phishing) (EventID: 214 from LetsDefend) |
| Date Investigated | 2026-07-15 |
| Event Time | Jan, 01, 2024, 12:37 PM |
| Verdict | True Positive |
| Time Spent | 31 mins |


## Trigger Reason

- New Year's Mandatory Security Update: Implementing Multi-Factor Authentication (MFA)


## Analyst Note

On Jan 01, 2024, at 12:37 PM, a SOC251 - Quishing Detected (QR Code Phishing) alert was triggered due to a QR code phishing attempt. After investigation, the alert was confirmed as a True Positive. Although the user scanned the QR code, the available logs do not provide any telemetry related to the scan. Furthermore, no suspicious processes or network connections were observed on the endpoint.


## Artifacts

- **Malicious SMTP Address** `158.69.201.47`
- **Sender Address** `security@microsecmfa.com`
- **QR code contain Malicious URL** `https://ipfs.io/ipfs/Qmbr8wmr41C35c3K2GfiP2F8YGzLhYpKpb4K66KU6mLmL4#`


## Threat Frameworks & Impact

- **MITRE ATT&CK:**
  - T1598.003
- **CVE:** N/A
- **Impact:** Medium


## Action Taken

- The affected host was contained.


## References

- **My Letsdefend Report:** https://app.letsdefend.io/case-management/casedetail/shakibul742/214 
- **Official MITRE ATT&CK:** https://attack.mitre.org/techniques/T1598/003/
- **Write-ups Reviewed After Investigation:** 
    - https://medium.com/@ezequiel.palacio/letsdefend-soc251-quishing-detected-qr-code-phishing-f823cffcf2b3
    
    - https://infosecwriteups.com/soc251-quishing-detected-qr-code-phishing-c6473454df7d