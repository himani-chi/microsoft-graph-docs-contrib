---
title: "macOSSoftwareUpdateDelayPolicy enum type"
description: "Flag enum to determine whether to delay software updates for macOS."
author: "jaiprakashmb"
ms.localizationpriority: medium
ms.subservice: "intune"
doc_type: enumPageType
ms.date: 08/01/2024
---

# macOSSoftwareUpdateDelayPolicy enum type

Namespace: microsoft.graph

> **Important:** APIs under the /beta version in Microsoft Graph are subject to change which could break your applications. While Intune /beta APIs are supported by Microsoft, you should use these at your own discretion. In general, /beta APIs are not recommended for use in production applications. To determine whether an API is available in v1.0, use the Version selector

> **Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.

Flag enum to determine whether to delay software updates for macOS.

## Members
|Member|Value|Description|
|:---|:---|:---|
|none|0|Software update delays will not be enforced.|
|delayOSUpdateVisibility|1|Force delays for OS software updates.|
|delayAppUpdateVisibility|2|Force delays for app software updates.|
|unknownFutureValue|4|Sentinel member for cases where the client cannot handle the new enum values.|
|delayMajorOsUpdateVisibility|8|Force delays for major OS software updates.|