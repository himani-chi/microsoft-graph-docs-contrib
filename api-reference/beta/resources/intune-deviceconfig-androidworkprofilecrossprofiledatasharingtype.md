---
title: "androidWorkProfileCrossProfileDataSharingType enum type"
description: "Android Work Profile cross profile data sharing type."
author: "jaiprakashmb"
ms.localizationpriority: medium
ms.subservice: "intune"
doc_type: enumPageType
ms.date: 08/01/2024
---

# androidWorkProfileCrossProfileDataSharingType enum type

Namespace: microsoft.graph

> **Important:** APIs under the /beta version in Microsoft Graph are subject to change which could break your applications. While Intune /beta APIs are supported by Microsoft, you should use these at your own discretion. In general, /beta APIs are not recommended for use in production applications. To determine whether an API is available in v1.0, use the Version selector

> **Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.

Android Work Profile cross profile data sharing type.

## Members
|Member|Value|Description|
|:---|:---|:---|
|deviceDefault|0|Device default value, no intent.|
|preventAny|1|Prevent any sharing.|
|allowPersonalToWork|2|Allow data sharing request from personal profile to work profile.|
|noRestrictions|3|No restrictions on sharing.|