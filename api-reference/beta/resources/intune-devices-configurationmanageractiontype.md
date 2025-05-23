---
title: "configurationManagerActionType enum type"
description: "Action type on Configuration Manager client"
author: "jaiprakashmb"
ms.localizationpriority: medium
ms.subservice: "intune"
doc_type: enumPageType
ms.date: 08/01/2024
---

# configurationManagerActionType enum type

Namespace: microsoft.graph

> **Important:** APIs under the /beta version in Microsoft Graph are subject to change which could break your applications. While Intune /beta APIs are supported by Microsoft, you should use these at your own discretion. In general, /beta APIs are not recommended for use in production applications. To determine whether an API is available in v1.0, use the Version selector

> **Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.

Action type on Configuration Manager client

## Members
|Member|Value|Description|
|:---|:---|:---|
|refreshMachinePolicy|0|Refresh machine policy on Configuration Manager client|
|refreshUserPolicy|1|Refresh user policy on Configuration Manager client|
|wakeUpClient|2|Wake up Configuration Manager client|
|appEvaluation|3|Evaluation application policy on Configuration Manager client|
|quickScan|5|Evaluation application policy on Configuration Manager client|
|fullScan|6|Evaluation application policy on Configuration Manager client|
|windowsDefenderUpdateSignatures|7|Evaluation application policy on Configuration Manager client|