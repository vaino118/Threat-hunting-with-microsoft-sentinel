# Threat Hunting with Microsoft Sentinel

## Project Overview

This project demonstrates a practical Security Operations Centre (SOC) threat hunting exercise using Microsoft Sentinel, Kusto Query Language (KQL), Sysmon and the MITRE ATT&CK Framework.

The project uses an Azure-hosted Windows 10 virtual machine to generate and collect security events. These events are analysed using Microsoft Sentinel to identify and investigate suspicious activities.

## Project Objectives

- Configure a Microsoft Sentinel threat hunting environment.
- Deploy and monitor a Windows 10 virtual machine hosted in Microsoft Azure.
- Collect and analyse Windows endpoint security events.
- Develop KQL queries to investigate suspicious activities.
- Apply the MITRE ATT&CK Framework to relevant threat hunting activities.
- Document investigation findings and detection evidence.

## Tools and Technologies

- Microsoft Azure
- Azure Virtual Machines
- Microsoft Sentinel
- Log Analytics Workspace
- Azure Monitor Agent (AMA)
- Kusto Query Language (KQL)
- Sysmon
- Windows 10
- MITRE ATT&CK Framework

## Project Architecture

The project uses an Azure-based environment consisting of a Windows 10 virtual machine, endpoint monitoring through Sysmon, log collection and Microsoft Sentinel for security analysis.

## Threat Hunting Methodology

The project follows these main stages:

1. Azure environment configuration.
2. Windows 10 virtual machine deployment.
3. Endpoint monitoring and log collection.
4. Threat hunting using KQL.
5. Investigation and analysis of suspicious activities.
6. Documentation of findings.

## Repository Structure

| Folder | Description |
|---|---|
| 01-Lab-Architecture | Lab architecture and design |
| 02-Environment-Setup | Azure, Sentinel and endpoint configuration |
| 03-Data-Collection | Log collection configuration |
| 04-Threat-Hunting | Threat hunting queries and techniques |
| 05-Investigation-Results | Investigation findings |
| 06-Screenshots | Supporting project evidence |

## Learning Outcomes

This project provided practical experience in:

- SIEM configuration and monitoring.
- Azure-based security monitoring.
- Windows endpoint event collection.
- KQL query development.
- Threat hunting techniques.
- MITRE ATT&CK mapping.
- Security investigation and documentation.

## Disclaimer

This project was conducted in a controlled cloud-based lab environment for educational and cybersecurity portfolio purposes.
