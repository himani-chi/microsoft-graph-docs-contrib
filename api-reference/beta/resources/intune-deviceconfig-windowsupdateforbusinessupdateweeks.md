---
title: "windowsUpdateForBusinessUpdateWeeks enum type"
description: "Scheduled the update installation on the weeks of the month"
author: "jaiprakashmb"
ms.localizationpriority: medium
ms.subservice: "intune"
doc_type: enumPageType
ms.date: 08/01/2024
---

# windowsUpdateForBusinessUpdateWeeks enum type

Namespace: microsoft.graph

> **Important:** APIs under the /beta version in Microsoft Graph are subject to change which could break your applications. While Intune /beta APIs are supported by Microsoft, you should use these at your own discretion. In general, /beta APIs are not recommended for use in production applications. To determine whether an API is available in v1.0, use the Version selector

> **Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.

Scheduled the update installation on the weeks of the month

## Members
|Member|Value|Description|
|:---|:---|:---|
|userDefined|0|Allow the user to set.|
|firstWeek|1|Scheduled the update installation on the first week of the month|
|secondWeek|2|Scheduled the update installation on the second week of the month|
|thirdWeek|4|Scheduled the update installation on the third week of the month|
|fourthWeek|8|Scheduled the update installation on the fourth week of the month|
|everyWeek|15|Scheduled the update installation on every week of the month|
|unknownFutureValue|22|Evolvable enum member|