# Suspicious Application Registration

## Overview
Detects anomalous or unauthorized application registrations in Entra ID, often used for persistence or privilege escalation.

## MITRE ATT&CK
- Technique: T1098.003 – Additional Cloud Credentials
- Tactics: Persistence, Privilege Escalation

## Data Sources
- Entra ID Audit Logs (ApplicationManagement)

## Tuning
- Exclude known admin and automation accounts
- Monitor service principal creation patterns
- Review app purpose with owners

## False Positives
- DevOps pipelines
- Legitimate admin testing

## Investigation
1. Identify who created the app.
2. Review recent sign-ins for that user.
3. Check assigned roles/permissions.
4. Validate business justification.
5. Review token issuance and usage.

## Automation Ideas
- Auto-enrich with user risk level.
- Auto-collect app metadata.
- Auto-flag high-privilege service principals.
