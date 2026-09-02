# Unauthorized Role Assignment

## Overview
Detects unauthorized or anomalous high-privilege role assignments in Entra ID.

## MITRE ATT&CK
- **Technique:** T1069.003 – Permission Groups Discovery (Cloud)
- **Tactic:** Privilege Escalation

## Data Sources
- Entra ID Audit Logs (RoleManagement)

## Use Case
Attackers escalate privileges by assigning themselves or compromised accounts to high-privilege roles.

## Tuning Guidance
- Exclude IAM admin accounts
- Validate legitimate change windows
- Monitor automation accounts

## False Positives
- Approved IAM changes
- Admin onboarding workflows

## Investigation Steps
1. Identify who assigned the role.
2. Validate the request through IAM change logs.
3. Review recent activity for the actor and target.
4. Check for privilege misuse.
5. Validate business justification.

## Recommended Automation
- Auto-enrich with role metadata.
- Auto-collect actor’s recent sign-ins.
- Auto-flag high-risk role assignments.
