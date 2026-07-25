## SOC127 - SQL Injection Detected

| Field | Value |
|---------|---------|
| Alert Name | SOC127 - SQL Injection Detected (EventID: 235 from LetsDefend) |
| Date Investigated | 2026-07-25 |
| Event Time | Mar, 07, 2024, 12:51 PM |
| Skill Level | Medium |
| Verdict | True Positive |
| Time Spent | 41 mins |


## Analyst Note

Dectected multiple sql injection through sqlmap tool.


## Artifacts

- **URL** `GET /?douj=3034 AND 1=1 UNION ALL SELECT 1,NULL,'<script>alert("XSS")</script>',table_name FROM information_schema.tables WHERE 2>1--/**/; EXEC xp_cmdshell('cat ../../../etc/passwd')# HTTP/1.1 200 865`
- **IP Address** `118.194.247.28`


## Threat Frameworks & Impact

- **MITRE ATT&CK:**
  - T1595 - Active Scanning (Reconnaissance)
- **CVE:** N/A
- **SEVERITY:** High


## Action Taken

- The affected host was contained.


## References

- **My Letsdefend Report:**
  - https://app.letsdefend.io/case-management/casedetail/shakibul742/235

- **Official MITRE ATT&CK:**
  - https://attack.mitre.org/techniques/T1595/

- **Write-ups Reviewed:**
  - https://medium.com/@RayxAB/soc-analysis-of-event-235-soc127-sql-injection-detected-lets-defend-b95f42e23a3c