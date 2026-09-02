# Privilege Escalation Workflow

## Objective
Investigate unauthorized role assignments or privilege elevation.

## Steps

### 1. Initial Triage
- Review Audit Logs
- Identify actor and target
- Validate change request

### 2. Indicators of Compromise
- Role assignment outside change window
- Actor with unusual sign-ins
- MFA disabled

### 3. Containment
- Remove unauthorized role
- Block actor account
- Revoke tokens

### 4. Investigation
- Review actor’s recent activity
- Check for lateral movement
- Validate business justification

### 5. Recovery
- Reassign correct roles
- Re-enable Conditional Access
- Reconfigure admin workflows

### 6. Reporting
- Document findings
- Provide RCA
