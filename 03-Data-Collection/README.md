# Data Collection and Log Ingestion

## 1. Overview

This section describes how endpoint security events were collected and forwarded to Microsoft Sentinel for threat hunting and investigation.

## 2. Data Collection Components

The following technologies were used:

- Azure Arc
- Azure Monitor Agent (AMA)
- Data Collection Rules (DCR)
- Log Analytics Workspace
- Microsoft Sentinel
- Sysmon

## 3. Log Collection Process

Sysmon was configured on the Windows 10 virtual machine to generate detailed endpoint activity logs.

Azure Monitor Agent was used to collect the configured Windows event logs.

Data Collection Rules defined the event sources and the destination for the collected data.

The collected logs were forwarded to the Log Analytics Workspace, which was connected to Microsoft Sentinel.

## 4. Event Monitoring

The project focused on collecting endpoint activities relevant to security monitoring and threat hunting, including:

- Process creation events.
- Windows security events.
- Failed login attempts.
- Suspicious process execution.
- Network connection activity.

## 5. Log Verification

The collected events were queried and analysed using Kusto Query Language (KQL) in Microsoft Sentinel.

This confirmed whether the required endpoint telemetry was available for threat hunting and investigation.

## 6. Objective

The objective was to establish reliable endpoint log collection and centralised security event monitoring using Microsoft Azure services.
