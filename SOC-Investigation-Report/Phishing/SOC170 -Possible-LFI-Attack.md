# SOC170 - Passwd Found in Requested URL - Possible LFI Attack

| Field             | Value                                                                                       |
| ----------------- | ------------------------------------------------------------------------------------------- |
| Alert Name        | SOC170 - Passwd Found in Requested URL - Possible LFI Attack (EventID: 120 from LetsDefend) |
| Date Investigated | 2026-06-17                                                                                  |
| Event Time        | Mar, 01, 2022, 10:10 AM                                                                     |
| Verdict           | True Positive                                                                               |
| Time Spent        | 43 mins                                                                                     |

## 1. Threat Frameworks & Impact

* **MITRE ATT&CK:**

  * T1190 – Exploit Public-Facing Application
* **Attack Type:** Local File Inclusion (LFI)
* **Impact:** Low (Attack Attempt Failed)

## 2. The Why (Core Evidence)

* The requested URL contained `../../../../etc/passwd`, a common LFI payload targeting sensitive Linux files.
* Web logs showed an **HTTP 500 Internal Server Error** with a **0-byte response**, indicating the file was not disclosed.
* The activity was a genuine LFI attack attempt but was unsuccessful.

## 3. Key IOCs

* **Source IP:** `106.55.45.162`
* **HTTP Method:** `GET`
* **Malicious URL:** `https://172.16.17.13/?file=../../../../etc/passwd`

## 4. Action Taken

* Documented the LFI attempt and confirmed that no sensitive file was exposed.
* No escalation or containment was required.