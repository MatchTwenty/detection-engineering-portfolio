# Privilege Escalation SOAR Playbook

## Trigger
- High-privilege role assignment
- Admin role added outside change window
- Privileged account suspicious activity

## Automated Actions
1. Pull Audit Logs for role assignment.
2. Identify actor and target.
3. Check actor’s recent sign-ins.
4. Revoke tokens for actor.
5. Remove role (pending approval).

## Human Approval Required
- Remove role
- Block actor account

## Enrichment
- Actor risk level
- Device compliance
- Conditional Access impact
- Role metadata

## Containment
- Remove unauthorized role
- Block actor account
- Revoke sessions

## Recovery
- Reassign correct roles
- Validate IAM workflows
- Re-enable Conditional Access

## Notifications
- IAM team
- Security operations
