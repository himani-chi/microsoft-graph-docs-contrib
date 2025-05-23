---
title: "vppTokenSyncStatus enum type"
description: "Possible sync statuses associated with an Apple Volume Purchase Program token."
author: "jaiprakashmb"
ms.localizationpriority: medium
ms.subservice: "intune"
doc_type: enumPageType
ms.date: 08/01/2024
---

# vppTokenSyncStatus enum type

Namespace: microsoft.graph

> **Important:** APIs under the /beta version in Microsoft Graph are subject to change which could break your applications. While Intune /beta APIs are supported by Microsoft, you should use these at your own discretion. In general, /beta APIs are not recommended for use in production applications. To determine whether an API is available in v1.0, use the Version selector

> **Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.

Possible sync statuses associated with an Apple Volume Purchase Program token.

## Members
|Member|Value|Description|
|:---|:---|:---|
|none|0|Default status.|
|inProgress|1|Last Sync in progress.|
|completed|2|Last Sync completed successfully.|
|failed|3|Last Sync failed.|