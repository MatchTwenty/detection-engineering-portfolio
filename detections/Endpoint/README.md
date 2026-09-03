# Endpoint Detections

This folder contains detections related to endpoint activity, including process execution, command-line usage, file system anomalies, and lateral movement. These detections help identify attacker tooling, exfiltration behavior, and suspicious remote access.

## Included Detections

- **Endpoint Lateral Movement Hunt**  
- **Rclone Command Line Usage**  
- **Renamed Rclone Binary**  
- **EsentUtl Alternative Data Stream Usage**  
- **WinSCP Command-Line Session Started**

## Data Sources

- DeviceProcessEvents  
- DeviceNetworkEvents  
- FileActivity Logs  
- Defender XDR Telemetry

## MITRE ATT&CK Coverage

- **T1021 — Remote Services**  
- **T1041 — Exfiltration Over C2 Channel**  
- **T1036 — Masquerading**  
- **T1564.004 — NTFS Alternate Data Streams**

