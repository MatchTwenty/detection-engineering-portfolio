# Cloud Identity Anomalies

## Overview
Detects unusual identity behavior across Azure and Entra ID, including abnormal sign-in volume, IP diversity, and audit activity.

## MITRE ATT&CK
- **Technique:** T1087 – Account Discovery
- **Tactics:** Discovery, Credential Access

## Data Sources
- Sign-In Logs
- Audit Logs

## Use Case
Attackers enumerate accounts and perform reconnaissance before privilege escalation or lateral movement.

## Tuning Guidance
- Exclude automation accounts
- Exclude known high-volume service accounts
- Validate expected audit activity

## False Positives
- Bulk admin operations
- Automated workflows

## Investigation Steps
1. Review sign-in patterns.
2. Check audit activity for anomalies.
3. Validate user behavior with the owner.
4. Review device and session details.
5. Check for privilege escalation attempts.

## Recommended Automation
- Auto-enrich with user risk level.
- Auto-collect audit event details.
