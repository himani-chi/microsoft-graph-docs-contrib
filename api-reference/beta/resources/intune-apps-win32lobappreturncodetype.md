---
title: "win32LobAppReturnCodeType enum type"
description: "Indicates the type of return code."
author: "jaiprakashmb"
ms.localizationpriority: medium
ms.subservice: "intune"
doc_type: enumPageType
ms.date: 08/01/2024
---

# win32LobAppReturnCodeType enum type

Namespace: microsoft.graph

> **Important:** APIs under the /beta version in Microsoft Graph are subject to change which could break your applications. While Intune /beta APIs are supported by Microsoft, you should use these at your own discretion. In general, /beta APIs are not recommended for use in production applications. To determine whether an API is available in v1.0, use the Version selector

> **Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.

Indicates the type of return code.

## Members
|Member|Value|Description|
|:---|:---|:---|
|failed|0|Failed.|
|success|1|Success.|
|softReboot|2|Soft-reboot is required.|
|hardReboot|3|Hard-reboot is required.|
|retry|4|Retry.|