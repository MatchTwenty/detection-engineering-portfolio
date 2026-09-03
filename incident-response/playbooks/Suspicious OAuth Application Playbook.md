# Suspicious OAuth Application SOAR Playbook

## Trigger
- New OAuth app created
- High-risk OAuth consent
- App requesting privileged scopes

## Automated Actions
1. Pull app metadata (publisher, permissions, creation time).
2. Identify actor who created/consented to the app.
3. Check for recent sign-ins by actor.
4. Revoke app tokens.
5. Disable app (pending approval).

## Human Approval Required
- Disable OAuth app
- Remove user consent

## Enrichment
- Permission scope analysis
- Token issuance history
- Actor risk level

## Containment
- Disable app
- Remove user consent
- Block actor account if compromised

## Recovery
- Re-enable legitimate apps
- Reconfigure Conditional Access
- Notify app owner if legitimate

## Notifications
- Identity team
- Security operations
