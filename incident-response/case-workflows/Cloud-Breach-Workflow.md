# Cloud Breach Workflow

## Objective
Investigate cloud compromise involving Azure, M365, or Entra ID.

## Steps

### 1. Initial Triage
- Review Sentinel alerts
- Check Identity Protection signals
- Validate user activity

### 2. Log Review
- Sign-In Logs
- Audit Logs
- Unified Audit Log
- Defender XDR alerts

### 3. Indicators of Compromise
- OAuth app creation
- Privilege escalation
- Token replay
- Unusual mailbox activity

### 4. Containment
- Block malicious apps
- Revoke tokens
- Disable compromised accounts

### 5. Investigation
- Review mailbox rules
- Check SharePoint/OneDrive access
- Review Teams activity
- Validate admin role changes

### 6. Recovery
- Reconfigure Conditional Access
- Re-enable MFA
- Restore mailbox or files

### 7. Reporting
- Document timeline
- Provide RCA
- Recommend cloud hardening
