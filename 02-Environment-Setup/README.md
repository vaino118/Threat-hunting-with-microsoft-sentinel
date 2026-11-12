# 🛡️ Environment Setup

## 1. Overview
This section describes the setup of the Microsoft Azure environment used for the threat hunting project.

## 2. Azure Infrastructure
The following components were configured:
- **Microsoft Azure** 
- **Windows 10 Virtual Machine** (Target Endpoint)
- **Azure Arc** (Hybrid server management)
- **Azure Monitor Agent (AMA)** (Log collection)
- **Log Analytics Workspace** (`LAW-SOC-ThreatHunting`)
- **Microsoft Sentinel** (SIEM)

## 3. Endpoint Configuration
A Windows 10 virtual machine was deployed in Microsoft Azure. 

**Sysmon** was installed to monitor endpoint activities and generate detailed system event logs (Event IDs 1, 3, 5, and 11) for deep threat hunting.

## 4. Security Monitoring
- **Azure Arc** and **Azure Monitor Agent** were configured to support machine management and log collection.
- **Data Collection Rules (DCRs)** were configured to define the events collected from the endpoint. *(Note: Due to Student subscription UI restrictions, the DCR for Sysmon was successfully deployed via Azure CLI/Cloud Shell).*
- **Microsoft Sentinel** was used to monitor and analyse the collected security events.

## 5. Objective
The purpose of this environment was to establish a centralised security monitoring platform for conducting threat hunting and investigating suspicious endpoint activities.
