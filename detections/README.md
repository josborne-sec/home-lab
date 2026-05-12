# Detection Engineering Portfolio

KQL detection rules built and validated in the Microsoft Sentinel Training Lab. Each rule includes the query, detection logic explanation, data source requirements, validation steps, and false positive considerations.

## Rules

| # | Detection | Tactic | Data Source |
|---|-----------|--------|-------------|
| 01 | Suspicious Mailbox Forwarding Rule | Collection | Exchange / Defender |
| 02 | Mass External Email Send | Exfiltration | Exchange / Defender |
| 03 | Impossible Travel | Initial Access | Entra ID Sign-in Logs |
| 04 | MFA Fatigue | Credential Access | Entra ID Sign-in Logs |
| 05 | Encoded PowerShell Execution | Execution | Defender for Endpoint |

## Environment

Built and tested using the Microsoft Sentinel Training Lab. KQL queries written against standard Microsoft 365 and Defender schemas.

## Background

These rules were written as portfolio examples. Detection logic is original work, written from scratch outside of any production environment.

## Structure

Each rule lives in its own folder containing:
- `[rule-name].kql` - the detection query
- `README.md` - detection writeup (logic, data sources, validation, FP tuning, response steps)
- `sample-events.json` - example event shape that triggers the rule
