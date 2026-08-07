##  SOC105 - Requested T.I. URL address

| Field | Value |
|---------|---------|
| Alert Name | SOC105 - Requested T.I. URL address (EventID: 75 from LetsDefend) |
| Date Investigated | 2026-07-28 |
| Event Time | Mar, 07, 2021, 05:47 PM |
| Skill Level | Easy |
| Verdict | False Positive |
| Time Spent | 35 mins |


## Analyst Note

On Mar, 07, 2021 at 05:47 PM the SOC105 - Requested T.I. URL address alert was triggered. The alert triggered reason was T.I Url address. But after investigation the url was legitimate, and no suspicious process was running. So the alert was false positive.


## Artifacts

- **Source Address** `10.15.15.12`
- **Destination Address** `67.199.248.10`
- **Url that triggered the alert** `https://bit.ly/TAPSCAN`


## Threat Frameworks & Impact

- **MITRE ATT&CK:**
  - N/A
- **CVE:** N/A
- **SEVERITY:** High


## Action Taken

- No action needed.


## References

- **Investigation Report (LetsDefend):**
  - https://app.letsdefend.io/case-management/casedetail/shakibul742/75

- **Write-ups Reviewed After Investigation:**
  - https://antoinemondange.medium.com/letsdefend-soc105-requested-t-i-url-address-ed3715df1e97