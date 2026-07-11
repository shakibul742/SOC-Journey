##  SOC250 - APT35 HyperScrape Data Exfiltration Tool Detected

| Field | Value |
|---------|---------|
| Alert Name | SOC250 - APT35 HyperScrape Data Exfiltration Tool Detected (EventID: 212 from LetsDefend) |
| Date Investigated | 2026-07-11 |
| Event Time | Dec, 27, 2023, 11:22 AM |
| Verdict | True Positive |
| Time Spent | 1h 28 mins |


## Trigger Reason

- Unusual or suspicious patterns of behavior linked to the hash have been identified, indicating potential malicious intent.


## Analyst Note

On Dec 27, 2023 at 11:22 AM, a SOC250 - APT35 HyperScrape Data Exfiltration Tool Detected alert was triggered. This alert was detected due to unusual or suspicious activity associated APT35 Charming Kitten. After investigation, the APT group successfully logged in through RDP (Source IP: 173.209.51.54, Logon Type: 10). The attacker then connected to the C2 server (c2 IP: 136.243.108.14) and executed the malicious process EmailDownloader.exe and performed multiple mail downloads. Therefore, this is a true positive alert. The affected user (Arthur) was contained.


## Artifacts

- **Malicious File Hash** `cd2ba296828660ecd07a36e8931b851dda0802069ed926b3161745aae9aa6daa`
- **Process Name** `EmailDownloader.exe`
- **Process Path** `C:\Users\LetsDefend\Downloads\EmailDownloader.exe`
- **Attacker IP** `173.209.51.54`
- **C2 IP** `136.243.108.14`


## Threat Frameworks & Impact

- **MITRE ATT&CK:**
  - TA453, COBALT ILLUSION, Charming Kitten, ITG18, Phosphorus, Newscaster, APT35, Mint Sandstorm
- **CVE:** N/A
- **Impact:** Medium


## Action Taken

- The affected user (Arthur) was contained.