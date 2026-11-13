# Threat Hunting with Microsoft Sentinel

## 1. Overview

This section documents the threat hunting activities conducted using Microsoft Sentinel and Kusto Query Language (KQL).

The objective was to identify, investigate and analyse suspicious endpoint activities collected from the Windows 10 virtual machine.

## 2. Threat Hunting Objectives

- Identify suspicious PowerShell execution.
- Investigate repeated failed login attempts.
- Detect suspicious account creation activities.
- Identify suspicious scheduled task creation.
- Investigate unusual process execution.
- Analyse potentially suspicious network connections.

## 3. MITRE ATT&CK Framework

The threat hunting activities were mapped to relevant MITRE ATT&CK techniques.

| Threat Activity | MITRE ATT&CK Technique |
|---|---|
| PowerShell execution | T1059.001 |
| Brute Force | T1110 |
| Account Creation | T1136 |
| Scheduled Task | T1053.005 |
| Command and Scripting Interpreter | T1059 |
| Application Layer Protocol | T1071 |

## 4. Threat Hunting Methodology

The following methodology was followed:

1. Define the threat hunting objective.
2. Identify relevant Windows security events.
3. Develop KQL queries.
4. Execute queries in Microsoft Sentinel.
5. Analyse returned results.
6. Document findings and supporting evidence.

## 5. Tools Used

- Microsoft Sentinel
- Log Analytics Workspace
- Kusto Query Language (KQL)
- Sysmon
- MITRE ATT&CK Framework

## 6. Results and Findings

The results of each threat hunting activity, including the KQL queries and supporting screenshots, are documented in this section.

## 7. Conclusion

The threat hunting exercises demonstrated how Microsoft Sentinel and KQL can be used to investigate endpoint activities and identify potentially suspicious behaviour.
