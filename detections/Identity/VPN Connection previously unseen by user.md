# VPN Connection Previously Unseen by User

## Overview
Detects VPN connections from IP ranges or geolocations not previously associated with the user.

## MITRE ATT&CK
- **Technique:** T1078 – Valid Accounts
- **Tactic:** Initial Access

## Data Sources
- VPN logs
- Sign-In Logs

## Use Case
Attackers often use stolen credentials to authenticate via VPN from new locations.

## Tuning Guidance
- Exclude known travel patterns
- Validate expected remote work behavior

## False Positives
- User travel
- New ISP or home network

## Investigation Steps
1. Review geolocation.
2. Check recent sign-in activity.
3. Validate user travel.
4. Review device compliance.
5. Check for MFA changes.

## Recommended Automation
- Auto-enrich with user risk.
- Auto-collect device info.
