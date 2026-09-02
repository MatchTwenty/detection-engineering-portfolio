# Rclone Command Line Usage

## Overview
Detects execution of Rclone with command-line arguments associated with cloud storage synchronization or data exfiltration.

## MITRE ATT&CK
- **Technique:** T1041 – Exfiltration Over Command and Control Channel
- **Tactic:** Exfiltration

## Data Sources
- DeviceProcessEvents
- CommandLine logs

## Use Case
Rclone is frequently used by attackers to exfiltrate data to cloud storage providers.

## Tuning Guidance
- Exclude legitimate backup tools
- Validate expected automation workflows

## False Positives
- Backup scripts
- DevOps automation

## Investigation Steps
1. Review command-line arguments.
2. Identify destination endpoints.
3. Check for large outbound transfers.
4. Validate user intent.
5. Review proxy/DLP logs.

## Recommended Automation
- Auto-enrich with file metadata.
- Auto-collect network transfer logs.
