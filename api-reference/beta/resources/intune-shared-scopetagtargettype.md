---
title: "scopeTagTargetType enum type"
description: "Specifies which type of Entra object to target in the Group for a given ScopeTag."
author: "jaiprakashmb"
ms.localizationpriority: medium
ms.subservice: "intune"
doc_type: enumPageType
ms.date: 08/01/2024
---

# scopeTagTargetType enum type

Namespace: microsoft.graph
> **Important:** APIs under the /beta version in Microsoft Graph are subject to change which could break your applications. While Intune /beta APIs are supported by Microsoft, you should use these at your own discretion. In general, /beta APIs are not recommended for use in production applications. To determine whether an API is available in v1.0, use the Version selector.

> **Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.


Specifies which type of Entra object to target in the Group for a given ScopeTag.

## Members
|Member|Value|Description|
|:---|:---|:---|
|none|0|Unused value. Do not use.|
|user|1|Indicates the ScopeTag assignment will Target Users in the Group Ids provided.|
|device|2|Indicates the ScopeTag assignment will Target Devices in the Group Ids provided.|
|unknownFutureValue|4|Evolvable enumeration sentinel value. Do not use.|
