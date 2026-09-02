# Insider Risk Behavioral Pattern

## Overview
Detects unusual file access behavior that may indicate insider threat activity or data exfiltration.

## MITRE ATT&CK
- **Technique:** T1041 – Exfiltration Over Command and Control Channel
- **Tactic:** Exfiltration

## Data Sources
- FileActivity logs
- DLP logs
- Proxy logs (optional)

## Use Case
Insider threats often download or copy large volumes of files before exfiltration.

## Tuning Guidance
- Exclude backup systems
- Exclude known high-volume service accounts
- Validate expected file access patterns

## False Positives
- Bulk data migrations
- System backups

## Investigation Steps
1. Identify user and file types accessed.
2. Review recent authentication activity.
3. Check for external uploads or transfers.
4. Validate business justification.
5. Review proxy/DLP logs for exfiltration.

## Recommended Automation
- Auto-enrich with file metadata.
- Auto-collect DLP alerts.
