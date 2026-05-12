# [Detection Name]

## Summary

One or two sentences: what this rule detects and why it matters.

## Threat Context

- **MITRE ATT&CK technique:** [TXXXX - Technique Name](https://attack.mitre.org/techniques/TXXXX/)
- **Tactic:** [Initial Access / Persistence / Collection / etc.]
- **Why this matters:** Brief plain-English explanation of the attacker behavior and what successful exploitation looks like.

## Detection Logic

Plain-language walkthrough of what the KQL does, step by step. Three to five sentences. No code in this section.

## Data Sources

- **Table:** [SigninLogs, DeviceProcessEvents, EmailEvents, etc.]
- **Required fields:** [list]
- **Required connectors:** [Entra ID, Defender for Endpoint, Office 365, etc.]

## Query

See [`[filename].kql`](./[filename].kql)

## Testing & Validation

How this was tested in the Microsoft Sentinel Training Lab. Specific lab scenario or simulated event used. Expected result when the rule fires.

## False Positive Considerations

- **[Known FP scenario 1]:** [tuning approach]
- **[Known FP scenario 2]:** [tuning approach]

## Response Recommendations

What an analyst should do when this rule fires. Investigation steps, pivots, escalation criteria.

## References

- [Microsoft documentation link]
- [Threat intel source]
- [Related MITRE ATT&CK reference]
