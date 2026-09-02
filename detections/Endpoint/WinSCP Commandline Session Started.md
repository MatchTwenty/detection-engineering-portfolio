# WinSCP Command-Line Session Started

## Overview
Detects command-line execution of WinSCP, which may indicate scripted file transfers or data exfiltration.

## MITRE ATT&CK
- **Technique:** T1041 – Exfiltration Over C2 Channel
- **Tactic:** Exfiltration

## Data Sources
- DeviceProcessEvents
- CommandLine logs

## Use Case
Attackers use WinSCP in scripted mode to automate data exfiltration.

## Tuning Guidance
- Validate legitimate automation
- Monitor unusual script usage

## False Positives
- Admin automation
- Backup scripts

## Investigation Steps
1. Review command-line arguments.
2. Identify remote destination.
3. Check for large outbound transfers.
4. Validate user intent.
5. Review proxy/DLP logs.

## Recommended Automation
- Auto-enrich with remote host metadata.
- Auto-collect network logs.

