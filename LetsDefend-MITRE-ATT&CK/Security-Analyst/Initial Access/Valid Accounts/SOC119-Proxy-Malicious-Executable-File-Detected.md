##  SOC119 - Proxy - Malicious Executable File Detected

| Field | Value |
|---------|---------|
| Alert Name | SOC119 - Proxy - Malicious Executable File Detected |
| EventID | 79 from LetsDefend |
| Date Investigated | 2026-08-07 |
| Event Time | Mar, 15, 2021, 09:30 PM |
| Type | Proxy |
| Skill Level | Easy |
| Verdict | False Positive |
| Time Spent | 53 mins |


## Analyst Note

On Mar 15, 2021 at 09:30 PM, the alert was triggered. After investigation, it was found that the user visited a GitHub tool page. However, the logs do not provide any evidence that the user downloaded or executed the tool. The URL accessed was https://github.com/BloodHoundAD/BloodHound/releases. Therefore, the alert was determined to be a false positive.


## Artifacts

- **Source Address** `172.16.20.5`
- **Destination Address** `140.82.121.4`
- **Url Address** `https://github.com/BloodHoundAD/BloodHound/releases`


## Threat Frameworks & Impact

- **MITRE ATT&CK:**
    - N/A
- **CVE:** N/A
- **SEVERITY:** Medium


## Action Taken

- No action needed.


## References

- **Write-ups Reviewed After Investigation:**
  - https://medium.com/@sarasheon/walkthrough-malicious-executable-file-detected-6a0437e8d9ea
  - https://www.youtube.com/watch?v=9blzHAEtd-I&list=PLf9uoZIIR1H3w9oTUcH00ynt4e7M1lAb3&index=62