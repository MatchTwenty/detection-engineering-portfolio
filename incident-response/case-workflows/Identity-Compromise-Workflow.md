# Identity Compromise Workflow

## Objective
Provide a structured workflow for investigating suspected identity compromise, credential misuse, or unauthorized authentication.

## Steps

### 1. Initial Triage
- Review alert details (IP, location, device, MFA status)
- Check Identity Protection risk signals
- Validate user activity with manager or user

### 2. Log Review
- Sign-In Logs
- Audit Logs
- Conditional Access logs
- MFA registration changes

### 3. Indicators of Compromise
- Impossible travel
- New device sign-ins
- MFA disabled or reset
- OAuth app consent anomalies

### 4. Containment
- Force password reset
- Revoke refresh tokens
- Block user temporarily
- Require MFA re-registration

### 5. Investigation
- Review recent activity (email, Teams, SharePoint)
- Check for privilege escalation
- Review mailbox rules
- Check OAuth app grants

### 6. Recovery
- Re-enable user access
- Reconfigure MFA
- Validate device compliance

### 7. Reporting
- Document timeline
- Identify root cause
- Recommend long-term controls
