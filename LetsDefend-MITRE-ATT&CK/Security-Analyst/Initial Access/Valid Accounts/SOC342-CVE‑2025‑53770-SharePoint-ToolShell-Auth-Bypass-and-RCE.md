## SOC342 - CVE-2025-53770 SharePoint ToolShell Auth Bypass and RCE

| Field             | Value                                                                     |
| ----------------- | ------------------------------------------------------------------------- |
| Alert Name        | SOC342 - CVE-2025-53770 SharePoint ToolShell Auth Bypass and RCE         |
| Event Id        | 320         |
| Date Investigated | 2026-08-10                                                                |
| Event Time        | Jul, 22, 2025, 01:07 PM                                                   |
| Type              | Web Attack                                                                 |
| Skill Level       | Hard                                                                      |
| Verdict           | True Positive                                                              |
| Time Spent        | 42 mins                                                            |

## Trigger Reason

- Suspicious unauthenticated POST request targeting SharePoint `ToolPane.aspx`.

## Analyst Note

On Jul, 22, 2025 at 01:07 PM, the alert was triggered by a suspicious POST request from external IP `107.191.58.76` targeting the SharePoint server `172.16.20.17`. The request targeted `/_layouts/15/ToolPane.aspx?DisplayMode=Edit&a=/ToolPane.aspx` with a large POST payload and `/layouts/SignOut.aspx` as the referer, indicating a CVE-2025-53770 ToolShell exploitation attempt.

Endpoint investigation confirmed successful exploitation. The SharePoint IIS worker process `w3wp.exe` spawned `powershell.exe` with an encoded command, confirming remote code execution. The attack was therefore confirmed as a **True Positive**.

## Artifacts

- **IP Address:** `107.191.58.76`
- **Destination IP Address:** `172.16.20.17`
- **File Name:** `spinstall0.aspx`
- **Process Name:** `powershell.exe`
- **Process Name:** `w3wp.exe`
- **Request URL:** `/_layouts/15/ToolPane.aspx?DisplayMode=Edit&a=/ToolPane.aspx`
- **Referer:** `/_layouts/SignOut.aspx`

## Threat Frameworks & Impact

- **MITRE ATT&CK:**
  - T1190 – Exploit Public-Facing Application
  - T1059.001 – Command and Scripting Interpreter: PowerShell
- **CVE:** CVE-2025-53770
- **Severity:** Critical
- **Impact:** Remote Code Execution

## Action Taken

- The affected SharePoint01 host was contained.
- The incident was escalated for further investigation and remediation.

## References

- **Investigation Report (LetsDefend):**
  - https://app.letsdefend.io/case-management/casedetail/shakibul742/320

- **CVE Details:**
  - https://nvd.nist.gov/vuln/detail/CVE-2025-53770

- **MITRE ATT&CK – Exploit Public-Facing Application:**
  - https://attack.mitre.org/techniques/T1190/

- **MITRE ATT&CK – PowerShell:**
  - https://attack.mitre.org/techniques/T1059/001/