---
title: "windowsSModeConfiguration enum type"
description: "The possible options to configure S mode unlock"
author: "jaiprakashmb"
ms.localizationpriority: medium
ms.subservice: "intune"
doc_type: enumPageType
ms.date: 08/01/2024
---

# windowsSModeConfiguration enum type

Namespace: microsoft.graph

> **Important:** APIs under the /beta version in Microsoft Graph are subject to change which could break your applications. While Intune /beta APIs are supported by Microsoft, you should use these at your own discretion. In general, /beta APIs are not recommended for use in production applications. To determine whether an API is available in v1.0, use the Version selector

> **Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.

The possible options to configure S mode unlock

## Members
|Member|Value|Description|
|:---|:---|:---|
|noRestriction|0|This option will remove all restrictions to unlock S mode - default|
|block|1|This option will block the user to unlock the device from S mode|
|unlock|2|This option will unlock the device from S mode|