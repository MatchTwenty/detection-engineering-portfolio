# Detection Index

A complete index of all detections in this repository, including KQL queries, JSON analytic rule templates, and Markdown documentation. Each entry includes its folder location and MITRE ATT&CK mapping.

---

## Identity Detections

| Detection Name | Folder | MITRE Technique | Description |
|----------------|--------|-----------------|-------------|
| **Suspicious Application Registration** | `Identity` | T1098.003 | Detects anomalous or unauthorized application registrations in Entra ID. |
| **Identity Misuse Detection** | `Identity` | T1078 | Detects unusual authentication patterns suggesting credential misuse. |
| **VPN Connection Previously Unseen by User** | `Identity` | T1078 | Detects VPN connections from new IP ranges or geolocations not previously associated with the user. |

---

## Privilege Escalation Detections

| Detection Name | Folder | MITRE Technique | Description |
|----------------|--------|-----------------|-------------|
| **Unauthorized Role Assignment** | `Privilege-escalation` | T1069.003 | Detects high‑privilege role assignments outside approved IAM workflows. |

---

## Cloud Security Detections

| Detection Name | Folder | MITRE Technique | Description |
|----------------|--------|-----------------|-------------|
| **Cloud Identity Anomalies** | `Cloud-Security` | T1087 | Detects unusual identity behavior across Azure/Entra ID. |

---

## Endpoint Detections

| Detection Name | Folder | MITRE Technique | Description |
|----------------|--------|-----------------|-------------|
| **Endpoint Lateral Movement Hunt** | `Endpoint` | T1021 | Identifies potential lateral movement via remote access tools. |
| **Rclone Command Line Usage** | `Endpoint` | T1041 | Detects Rclone execution with exfiltration‑related command‑line arguments. |
| **Renamed Rclone Binary** | `Endpoint` | T1036, T1041 | Detects Rclone executed under a renamed binary to evade detection. |
| **EsentUtl Alternative Data Stream Usage** | `Endpoint` | T1564.004 | Detects EsentUtl.exe interacting with NTFS Alternate Data Streams. |
| **WinSCP Command-Line Session Started** | `Endpoint` | T1041 | Detects scripted WinSCP command‑line sessions used for automated file transfers or exfiltration. |

---

## Behavioral / Insider Risk Detections

| Detection Name | Folder | MITRE Technique | Description |
|----------------|--------|-----------------|-------------|
| **Insider Risk Behavioral Pattern** | `Behavioral` | T1041 | Detects unusual file access behavior suggesting insider threat or exfiltration. |

---

## MITRE Coverage Summary

| Tactic | Techniques Covered |
|--------|--------------------|
| **Initial Access** | T1078 |
| **Privilege Escalation** | T1069.003 |
| **Persistence** | T1098.003 |
| **Defense Evasion** | T1036, T1564.004 |
| **Discovery** | T1087 |
| **Lateral Movement** | T1021 |
| **Exfiltration** | T1041 |

---

## How to Use This Index

Each detection includes:

- `.kql` — the detection query  
- `.json` — Sentinel analytic rule template  
- `.md` — documentation, tuning guidance, investigation steps  
