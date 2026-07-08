# SOC257 - VPN Connection Detected from Unauthorized Country

| Field | Value |
|---------|---------|
| Alert Name | SOC257 - VPN Connection Detected from Unauthorized Country (EventID: 225 from LetsDefend) |
| Date Investigated | 2026-07-08 |
| Event Time | Feb, 13, 2024, 02:04 AM |
| Verdict | True Positive |
| Time Spent | 1h 35 mins |

## Analyst Note

Investigation determined this alert is a True Positive. Firewall, VPN authentication, OS, and proxy logs were reviewed. Multiple failed VPN login attempts originated from source IP 113.161.158.12 against the VPN server (33.33.33.33). The attacker enumerated several usernames before successfully authenticating as mane@letsdefend.io. The successful login originated from an unauthorized country, indicating compromised user credentials. No evidence of malware, persistence, or additional malicious activity on the endpoint was identified. The affected account should have its password reset, MFA enabled if available, and future VPN logins from this source IP or region should be monitored or blocked.

## Threat Frameworks & Impact

- **MITRE ATT&CK:**
  - 
- **CVE:** N/A
- **Impact:** Medium

## The "Why" (Core Evidence)

- Vpn Connection Detected from Unauthorized Country

## Key IOCs

- **Unauthorized vpn souce ip** `113.161.158.12`
- **VPN server destination** `33.33.33.33`

## Action Taken

- No action needed.