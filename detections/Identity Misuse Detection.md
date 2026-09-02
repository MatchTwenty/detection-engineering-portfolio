# Identity Misuse Detection

## Overview
This detection identifies unusual authentication patterns that may indicate credential misuse, account compromise, or unauthorized access.

## MITRE ATT&CK
- **Technique:** T1078 – Valid Accounts  
- **Tactics:** Initial Access, Credential Access

## Data Sources
- Azure AD Sign-In Logs

## Use Case
Attackers often use stolen credentials to authenticate from multiple IPs, geographies, or devices within short time windows.

## Tuning Guidance
- Exclude VPN ranges
- Exclude known admin travel patterns
- Combine with Identity Protection risk signals

## False Positives
- International travel
- Shared admin accounts
- VPN load balancers

## Investigation Steps
1. Review sign-in locations and IPs.
2. Check recent password resets or MFA changes.
3. Validate user travel or activity.
4. Review device compliance and risk.
5. Check for impossible travel alerts.

## Recommended Automation
- Auto-enrich with user risk level.
- Auto-collect device info.
- Auto-flag high-risk sign-ins.
