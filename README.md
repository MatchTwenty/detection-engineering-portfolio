# Detections Library

This folder contains high-fidelity detection rules written in Kusto Query Language (KQL), each paired with a JSON analytic rule template and a Markdown documentation file. The goal of this library is to demonstrate mature, production-ready detection engineering practices aligned with Microsoft Sentinel, Azure Data Explorer (ADX), and MITRE ATT&CK.

## Structure

Detections are organized into the following categories:

- **identity/** — Authentication anomalies, account misuse, OAuth abuse, and identity-based threats  
- **privilege-escalation/** — Unauthorized role assignments, admin elevation, and IAM abuse  
- **cloud-security/** — Azure/M365 cloud threat detections  
- **endpoint/** — Process, command-line, file system, and lateral movement detections  
- **behavioral/** — Insider threat, anomaly-based detections, and behavioral analytics  

Each detection includes:

- `.kql` — Detection query  
- `.json` — Sentinel analytic rule template  
- `.md` — Documentation, tuning guidance, investigation steps  

See `detections-index.md` for a full list of detections.

