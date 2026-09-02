# Renamed Rclone Binary

## Overview
Detects execution of Rclone when renamed to bypass security controls or signature-based detection.

## MITRE ATT&CK
- **Technique:** T1036 – Masquerading  
- **Technique:** T1041 – Exfiltration Over C2 Channel  
- **Tactics:** Defense Evasion, Exfiltration

## Data Sources
- DeviceProcessEvents

## Use Case
Attackers frequently rename Rclone to blend in with legitimate binaries.

## Tuning Guidance
- Validate expected admin tools
- Monitor unusual binary names

## False Positives
- Custom admin utilities
- Renamed backup tools

## Investigation Steps
1. Identify binary hash.
2. Compare against known Rclone signatures.
3. Review command-line arguments.
4. Check for outbound transfers.
5. Validate user intent.

## Recommended Automation
- Auto-enrich with file hash reputation.
- Auto-collect network logs.
