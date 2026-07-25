# SOC Analyst Portfolio

<p align="center">
  Hands-on LetsDefend investigations, structured around the MITRE ATT&CK framework.
</p>

<p align="center">
  <strong>Current focus:</strong> Security Analyst (Tier 1) &nbsp;|&nbsp; <strong>Next track:</strong> Incident Responder
</p>

---

## Portfolio Direction

This repository documents practical SOC investigations completed in LetsDefend's simulated environment. New work follows the official MITRE ATT&CK sequence so that each investigation builds into a clear, role-based learning path.

| Current | Next | Archive |
| :--- | :--- | :--- |
| **Security Analyst (Tier 1)**<br>MITRE ATT&CK-aligned investigations, completed sequentially. | **Incident Responder**<br>Will be added after the Tier 1 path is complete. | **SOC Investigation Report**<br>Previously solved alerts, retained in their original type-based categories. |

## Learning Roadmap

```text
Security Analyst (Tier 1)                         Incident Responder
            │                                              │
            ▼                                              ▼
MITRE ATT&CK-aligned investigations  ───────►  Added after Tier 1 is complete
            │
            ▼
Previously solved matching reports are moved from the legacy archive as needed
```

## Repository Structure

```text
SOC-Journey/
│
├── Letsdefend-MITRE-ATT&CK/                    # Active learning path
│   ├── Security-Analyst/                        # Current: Tier 1
│   │   ├── Reconnaissance/
│   │   │   ├── Active-Scanning/
│   │   │   └── Gather Victim Identity Information/
│   │   └── Resource Development/
│   │       └── Compromise Accounts/
│   │
│   └── Incident-Responder/                      # Planned after Tier 1
│
├── SOC-Investigation-Report/                    # Existing solved-alert archive
│   ├── Brute Force/
│   ├── Phishing/
│   ├── Powershell/
│   ├── ThreatIntel/
│   └── Web-Attack/
│       ├── IDOR/
│       ├── LFI-RFI/
│       ├── LS/
│       └── XSS/
│
└── README.md
```

> `Incident-Responder/` is the planned second track. All other paths shown reflect the current repository structure.

## Active Track

| Path | Scope | Progress |
| :--- | :--- | :--- |
| **[LetsDefend MITRE ATT&CK](./Letsdefend-MITRE-ATT%26CK/)** | The primary MITRE ATT&CK-based learning structure. | Active |
| **[Security Analyst](./Letsdefend-MITRE-ATT%26CK/Security-Analyst/)** | Tier 1 investigations, organized and completed in sequence. | In progress |
| **Incident Responder** | Incident-response investigations under the same framework. | Planned |

## Existing Solved Reports

The [SOC Investigation Report](./SOC-Investigation-Report/) directory is the current archive of alerts solved before this MITRE ATT&CK-based organization was introduced. Its contents will stay in place for now.

When progressing through the active track, an investigation that already exists in this archive will be moved to its relevant MITRE ATT&CK technique folder. This keeps the new structure sequential without duplicating reports.

| Archive category | Coverage |
| :--- | :--- |
| **[Web Attacks](./SOC-Investigation-Report/Web-Attack/)** | HTTP analysis, XSS, LFI, IDOR, and command injection. |
| **[Phishing](./SOC-Investigation-Report/Phishing/)** | Malicious emails, URLs, attachments, and DLL side-loading. |
| **[Brute Force](./SOC-Investigation-Report/Brute%20Force/)** | RDP login anomalies and account-compromise validation. |
| **[PowerShell](./SOC-Investigation-Report/Powershell/)** | Suspicious script execution and command-and-control activity. |
| **[Threat Intelligence](./SOC-Investigation-Report/ThreatIntel/)** | Domain, reputation, and other threat-intelligence investigations. |

## Investigation Approach

```text
Alert Review  →  Log Analysis  →  Validation  →  Classification  →  Remediation
```

**Focus areas:** alert triage, SIEM investigation, log analysis, threat intelligence, MITRE ATT&CK mapping, and incident response.

**Environment and tools:** LetsDefend, SIEM, VirusTotal, Any.Run, ExifTool, Volatility, URLhaus, AbuseIPDB, Cisco Talos, and WHOIS.

---

<sub>All investigations in this repository are conducted in safe, simulated lab environments. No real-world corporate or personal data is involved.</sub>
