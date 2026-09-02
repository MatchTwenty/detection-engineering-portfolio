# Detection Engineering Library

This folder contains high-fidelity detection rules written in Kusto Query Language (KQL) for Microsoft Sentinel and Azure Data Explorer (ADX). Each detection includes:

- A KQL query
- Metadata (MITRE ATT&CK, severity, data sources)
- A JSON analytic rule template (Detection-as-Code)
- A markdown explanation file
- Tuning guidance and false positive considerations
- Investigation steps and enrichment recommendations

## Folder Structure

- **identity/**  
  Detections related to identity misuse, authentication anomalies, privilege abuse, and Entra ID activity.

- **privilege-escalation/**  
  Detections for role changes, admin elevation, and unauthorized privilege assignments.

- **cloud-security/**  
  Azure, M365, and cloud workload detections.

- **endpoint/**  
  Endpoint-based detections (CrowdStrike, Defender, Windows artifacts).

- **behavioral/**  
  Behavioral analytics, anomaly detection, insider-risk patterns.

## Detection Format

Each detection includes:
- `.kql` — the query  
- `.json` — Sentinel analytic rule template  
- `.md` — documentation and tuning guidance  

See `detections-index.md` for a full list of detections.
