---
title: "appLockerApplicationControlType enum type"
description: "Possible values of AppLocker Application Control Types"
author: "jaiprakashmb"
ms.localizationpriority: medium
ms.subservice: "intune"
doc_type: enumPageType
ms.date: 08/01/2024
---

# appLockerApplicationControlType enum type

Namespace: microsoft.graph

> **Important:** APIs under the /beta version in Microsoft Graph are subject to change which could break your applications. While Intune /beta APIs are supported by Microsoft, you should use these at your own discretion. In general, /beta APIs are not recommended for use in production applications. To determine whether an API is available in v1.0, use the Version selector

> **Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.

Possible values of AppLocker Application Control Types

## Members
|Member|Value|Description|
|:---|:---|:---|
|notConfigured|0|Device default value, no Application Control type selected.|
|enforceComponentsAndStoreApps|1|Enforce Windows component and store apps.|
|auditComponentsAndStoreApps|2|Audit Windows component and store apps.|
|enforceComponentsStoreAppsAndSmartlocker|3|Enforce Windows components, store apps and smart locker.|
|auditComponentsStoreAppsAndSmartlocker|4|Audit Windows components, store apps and smart locker​.|