# SOC176 - RDP Brute Force Detected

| Field | Value |
|---------|---------|
| Alert Name | SOC176 - RDP Brute Force Detected (EventID: 234 from LetsDefend) |
| Date Investigated | 2026-07-07 |
| Event Time | Mar, 07, 2024, 11:44 AM |
| Verdict | True Positive |
| Time Spent | 1h 12 mins |

## Analyst Note

The SOC176 - RDP Brute Force Detected alert was triggered on Mar 07, 2024 at 11:44 AM due to multiple failed RDP login attempts from a single external ip address. The investigation confirmed the alert as a True positive with a Medium impact. The attacker attempted to authenticate using multiple usernames (admin, guest, sysadmin, Matthew) within one minute. The first three attempts failed (Event ID 4625), while the Matthew account successfully authenticated via RDP (Event ID 4624, Logon Type 10), confirming that the account was compromised. The compromised account was immediately contained.

## Threat Frameworks & Impact

- **MITRE ATT&CK:**
  - 1110.001 – Brute Force: Password Guessing
  - T1021.001 – Remote Services: Remote Desktop Protocol
- **CVE:** N/A
- **Impact:** Medium

## The "Why" (Core Evidence)

- Login failure from a single source with different non existing accounts

## Key IOCs

- **Attacker Ip Address** `218.92.0.56`
- **Brute Force attempted usernames** `admin, guest, sysadmin, Matthew`
- **Compromised Account** `Matthew`

## Action Taken

- Contained the compromised user account (**Matthew**) to prevent further malicious activity.