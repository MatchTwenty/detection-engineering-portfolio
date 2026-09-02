# EsentUtl Alternative Data Stream Usage

## Overview
Detects usage of EsentUtl.exe to create or manipulate NTFS Alternate Data Streams (ADS), a common defense evasion technique.

## MITRE ATT&CK
- **Technique:** T1564.004 – Hide Artifacts: NTFS Alternate Data Streams
- **Tactic:** Defense Evasion

## Data Sources
- DeviceProcessEvents
- FileActivity logs

## Use Case
Attackers hide malicious payloads or exfiltration staging files inside ADS.

## Tuning Guidance
- Validate legitimate forensic use
- Monitor admin tool usage

## False Positives
- Forensic investigations
- Backup utilities

## Investigation Steps
1. Review ADS path.
2. Identify user and process context.
3. Check for hidden payloads.
4. Review file metadata.
5. Validate business justification.

## Recommended Automation
- Auto-enrich with file metadata.
- Auto-collect ADS details.
