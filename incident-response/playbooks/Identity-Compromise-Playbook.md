# Identity Compromise SOAR Playbook

## Trigger
- Impossible travel alert
- High-risk sign-in
- MFA disabled/reset
- OAuth app consent anomaly

## Automated Actions
1. Collect last 24 hours of sign-in logs.
2. Collect Identity Protection risk signals.
3. Revoke refresh tokens.
4. Force password reset (pending approval).
5. Gather device compliance status.
6. Check for mailbox rule creation.

## Human Approval Required
- Force password reset
- Temporary user block

## Enrichment
- Geo-IP lookup
- Device risk score
- MFA registration history
- OAuth app metadata

## Containment
- Block user (optional)
- Revoke sessions
- Disable suspicious OAuth apps

## Recovery
- Re-enable MFA
- Validate device compliance
- Restore mailbox rules if needed

## Notifications
- Security team
- User’s manager
