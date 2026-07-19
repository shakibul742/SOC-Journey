##  SOC326 - Impersonating Domain MX Record Change Detected

| Field | Value |
|---------|---------|
| Alert Name | SOC326 - Impersonating Domain MX Record Change Detected (EventID: 304 from LetsDefend) |
| Date Investigated | 2026-07-18 |
| Event Time | Sep, 17, 2024, 12:05 PM |
| Verdict | True Positive |
| Time Spent | 1h  22 mins |


## Trigger Reason

- The MX record of a suspicious domain was changed, suggesting potential phishing activity.


## Analyst Note

The alert was triggered because an impersonating domain (letsdefwnd.io) was configured with an MX record to support phishing emails. A phishing email from [voucher@letsdefwnd.io](mailto:voucher@letsdefwnd.io) was delivered to the user, and investigation confirmed the user accessed the malicious link. The endpoint was contained, and the malicious email, domain, and IP were blocked. The alert was confirmed as a True Positive.


## Artifacts

- **Attacker IP** `45.33.23.183`
- **Domain** `letsdefwnd[.]io`


## Threat Frameworks & Impact

- **MITRE ATT&CK:**
  - T1656 – Impersonation
  - T1566 – Phishing
  - T1598.003 – Spearphishing Link
- **CVE:** N/A
- **Impact:** Medium


## Action Taken

- The affected host (mateo) was contained.
- The phishing email was removed.


## References

- **My Letsdefend Report:**
  - https://app.letsdefend.io/case-management/casedetail/shakibul742/304

- **Official MITRE ATT&CK:**
  - https://attack.mitre.org/techniques/T1656/
  - https://attack.mitre.org/techniques/T1566/
  - https://attack.mitre.org/techniques/T1598/003/

- **Write-ups Reviewed:**
  - https://medium.com/@corlissS/letsdefend-soc326-impersonating-domain-mx-record-change-detected-d1e17704f9b5