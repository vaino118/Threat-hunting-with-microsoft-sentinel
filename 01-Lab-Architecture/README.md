# Lab Architecture

## Overview

The lab environment was built using Microsoft Azure to demonstrate endpoint monitoring, security log collection and threat hunting using Microsoft Sentinel.

A Windows 10 virtual machine hosted in Azure was configured with Sysmon to generate detailed endpoint activity logs.

Azure Arc was installed to enable machine management, while Azure Monitor Agent (AMA) was used to collect logs according to the configured Data Collection Rules (DCRs).

## Architecture Components

| Component | Purpose |
|---|---|
| Microsoft Azure | Cloud infrastructure hosting the lab |
| Windows 10 VM | Endpoint used for security monitoring and testing |
| Sysmon | Generates detailed Windows system activity logs |
| Azure Arc | Provides connected machine management |
| Azure Monitor Agent | Collects configured endpoint events |
| Data Collection Rules | Define which events are collected |
| Log Analytics Workspace | Stores collected security logs |
| Microsoft Sentinel | Provides security monitoring and threat hunting using KQL |

## Log Collection Workflow

1. Sysmon generates endpoint activity events.
2. Azure Monitor Agent collects the configured events.
3. Data Collection Rules determine which events are forwarded.
4. Logs are sent to the Log Analytics Workspace.
5. Microsoft Sentinel is used to query and investigate the collected events.

Azure Arc provides the connected machine management layer and is not itself the log storage or analysis component.

## Objective

The architecture provides a cloud-based environment for collecting endpoint telemetry and conducting practical security threat hunting.
