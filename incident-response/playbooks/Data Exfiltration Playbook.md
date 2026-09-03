# Data Exfiltration SOAR Playbook

## Trigger
- Large file downloads
- External uploads
- DLP alerts
- Suspicious Rclone/WinSCP usage

## Automated Actions
1. Collect file access logs.
2. Pull DLP alert metadata.
3. Review proxy logs for outbound transfers.
4. Block external sharing (pending approval).
5. Identify user and device involved.

## Human Approval Required
- Block external sharing
- Temporary user suspension

## Enrichment
- File metadata
- User behavior history
- Device risk score
- Network transfer volume

## Containment
- Disable external sharing
- Block user temporarily
- Kill exfiltration processes (Rclone, WinSCP)

## Recovery
- Restore legitimate access
- Implement least privilege
- Add monitoring rules

## Notifications
- Data governance team
- Security leadership
