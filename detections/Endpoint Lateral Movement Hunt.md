# Endpoint Lateral Movement Hunt

## Overview
Detects potential lateral movement using remote access protocols such as RDP, SSH, and WinRM.

## MITRE ATT&CK
- **Technique:** T1021 – Remote Services
- **Tactic:** Lateral Movement

## Data Sources
- DeviceNetworkEvents
- ProcessCreation logs

## Use Case
Attackers pivot across endpoints using remote access tools after initial compromise.

## Tuning Guidance
- Exclude known IT admin tools
- Validate remote management workflows
- Monitor unusual process names

## False Positives
- IT support activity
- Automation scripts

## Investigation Steps
1. Identify initiating process.
2. Review remote IP reputation.
3. Check user context and privileges.
4. Validate remote access purpose.
5. Review endpoint telemetry for anomalies.

## Recommended Automation
- Auto-enrich with device risk.
- Auto-collect process metadata.
