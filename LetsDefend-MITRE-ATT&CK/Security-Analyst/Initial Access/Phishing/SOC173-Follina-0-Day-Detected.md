##  SOC173 - Follina 0-Day Detected

| Field | Value |
|---------|---------|
| Alert Name | SOC173 - Follina 0-Day Detected (EventID: 123 from LetsDefend) |
| Date Investigated | 2026-08-02 |
| Event Time | Jun, 02, 2022, 03:22 PM |
| Type | Malware |
| Skill Level | Hard |
| Verdict | True Positive |
| Time Spent | 47 mins |


## Trigger Reason

- msdt.exe executed after Office document


## Analyst Note

On Jun, 02, 2022 at 03:22 PM the alert was triggered by a phishing email containing the malicious attachment (05-2022-0438.doc). The user opend the attachment, which exploited the vulnerability and executed msdt.exe to retrieve RDF842l.html from the C2 server (www.xmlformats.com / 141.105.65.149). Proxy and firewall logs confirmed the C2 server connection. Therefore, the alert was  confirmed as a True Positive.


## Artifacts

- **File Name** `05-2022-0438.doc`
- **File Hash** `52945af1def85b171870b31fa4782e52`
- **Process Name** `msdt.exe`
- **Ip Address** `141.105.65.149`
- **Url Address** `www.xmlformats.com/office/word/2022/wordprocessingDrawing/RDF842I.html`
- **E-mail Address** `radiosputnik@ria.ru`


## Threat Frameworks & Impact

- **MITRE ATT&CK:**
    - T1566.001 – Phishing: Spearphishing Attachment
    - T1203 - Exploitation for Client Execution
- **CVE:** CVE-2022-30190
- **SEVERITY:** Medium


## Action Taken

- The affected host (JonasPRD) was contained.
- The phishing email was removed.


## References

- **Official MITRE ATT&CK:**
  - https://attack.mitre.org/techniques/T1566/001/
  - https://attack.mitre.org/techniques/T1203/

- **Letsdefend Official Write-up Reviewed After Investigation:**
  - https://download.cyberlearn.academy/download/download?url=https://files-ld.s3.us-east-2.amazonaws.com/Alert-Reports/follina_0day_detected.pdf