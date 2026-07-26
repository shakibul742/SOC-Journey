##  SOC325 - Unauthorized Cloud Region Access Attempt Detected

| Field | Value |
|---------|---------|
| Alert Name | SOC325 - Unauthorized Cloud Region Access Attempt Detected (EventID: 303 from LetsDefend) |
| Date Investigated | 2026-07-25 |
| Event Time | Sep, 24, 2024, 08:21 AM |
| Skill Level | Easy |
| Verdict | True Positive |
| Time Spent | 1h 15 mins |


## Trigger Reason

- Too many access attempts with the same user were detected in a short period of time from an unauthorized (configured as “unused” or “unsupported”) cloud region.


## Analyst Note

On Sep 24, 2024, at 08:21 AM, the SOC325 - Unauthorized Cloud Region Access Attempt Detected alert was triggered. The investigation revealed multiple unauthorized cloud region access attempts, indicating a brute-force attack. Log and endpoint investigations confirmed that all attempts were unsuccessful. Therefore, the alert was classified as a True Positive.


## Artifacts

- **Attacker IP** `134.209.145.73`


## Threat Frameworks & Impact

- **MITRE ATT&CK:**
  - T1586 - Compromise Accounts
  - T1110 - Brute Force
  - T1535: Unused/Unsupported Cloud Regions
  - T1078: Valid Accounts (Initial Access)
- **CVE:** N/A
- **SEVERITY:** Low


## Action Taken

- No action needed.


## References

- **My LetsDefend Report:** 
  - https://app.letsdefend.io/case-management/casedetail/shakibul742/303

- **Official MITRE ATT&CK:** 
  - https://attack.mitre.org/techniques/T1586/
  - https://attack.mitre.org/techniques/T1110/
  - https://attack.mitre.org/techniques/T1535/
  - https://attack.mitre.org/techniques/T1078/

  - **Write-ups Reviewed After Investigation:**
    - https://medium.com/@adeyemiaayatullah/eventid-303-soc325-unauthorized-cloud-region-access-attempt-detected-dd626a61fde8