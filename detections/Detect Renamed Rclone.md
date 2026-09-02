# Suspicious Application Registration

## Overview
This detection identifies anomalous or unauthorized application registrations in Entra ID, which may indicate credential theft, privilege escalation, or persistence mechanisms.

## MITRE ATT&CK
- **Technique:** T1098.003 – Additional Cloud Credentials  
- **Tactics:** Persistence, Privilege Escalation

## Data Sources
- Entra ID Audit Logs
- Service Principal Creation Events

## Use Case
Attackers frequently register malicious applications to obtain OAuth tokens, escalate privileges, or maintain persistence.

## Tuning Guidance
- Exclude known admin activity
- Monitor service principal creation patterns
- Validate legitimate automation workflows

## False Positives
- Legitimate DevOps automation
- Admin testing activity

## Investigation Steps
1. Identify the user who created the app
2. Review recent authentication activity
3. Check for privilege assignments
4. Validate app purpose with the owner
5. Review token issuance logs

## Recommended Automation
- Auto-enrich with user risk level
- Auto-collect app metadata
- Auto-flag high-risk service principals
