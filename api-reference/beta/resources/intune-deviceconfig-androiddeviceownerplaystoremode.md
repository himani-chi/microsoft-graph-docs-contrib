---
title: "androidDeviceOwnerPlayStoreMode enum type"
description: "Android Device Owner Play Store mode type."
author: "jaiprakashmb"
ms.localizationpriority: medium
ms.subservice: "intune"
doc_type: enumPageType
ms.date: 08/01/2024
---

# androidDeviceOwnerPlayStoreMode enum type

Namespace: microsoft.graph

> **Important:** APIs under the /beta version in Microsoft Graph are subject to change which could break your applications. While Intune /beta APIs are supported by Microsoft, you should use these at your own discretion. In general, /beta APIs are not recommended for use in production applications. To determine whether an API is available in v1.0, use the Version selector

> **Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.

Android Device Owner Play Store mode type.

## Members
|Member|Value|Description|
|:---|:---|:---|
|notConfigured|0|Not Configured|
|allowList|1|Only apps that are in the policy are available and any app not in the policy will be automatically uninstalled from the device.|
|blockList|2|All apps are available and any app that should not be on the device should be explicitly marked as 'BLOCKED' in the applications policy.|