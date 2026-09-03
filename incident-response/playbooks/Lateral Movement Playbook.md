# Lateral Movement SOAR Playbook

## Trigger
- RDP/SSH/WinRM anomalies
- Multiple remote connections
- Suspicious process initiating remote sessions

## Automated Actions
1. Collect DeviceNetworkEvents.
2. Pull process tree for initiating process.
3. Identify remote hosts involved.
4. Isolate device (pending approval).
5. Block remote IP if malicious.

## Human Approval Required
- Device isolation
- IP blocking

## Enrichment
- Remote host reputation
- User privilege level
- Device risk score

## Containment
- Isolate device
- Kill remote access processes
- Block malicious IPs

## Recovery
- Restore device access
- Reimage if needed
- Validate user permissions

## Notifications
- Endpoint team
- SOC leadership
