---
title: "androidRequiredPasswordComplexity enum type"
description: "The password complexity types that can be set on Android. One of: NONE, LOW, MEDIUM, HIGH. This is an API targeted to Android 11+."
author: "jaiprakashmb"
ms.localizationpriority: medium
ms.subservice: "intune"
doc_type: enumPageType
ms.date: 08/01/2024
---

# androidRequiredPasswordComplexity enum type

Namespace: microsoft.graph

> **Important:** APIs under the /beta version in Microsoft Graph are subject to change which could break your applications. While Intune /beta APIs are supported by Microsoft, you should use these at your own discretion. In general, /beta APIs are not recommended for use in production applications. To determine whether an API is available in v1.0, use the Version selector

> **Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.

The password complexity types that can be set on Android. One of: NONE, LOW, MEDIUM, HIGH. This is an API targeted to Android 11+.

## Members
|Member|Value|Description|
|:---|:---|:---|
|none|0|Device default value, no password.|
|low|1|The required password complexity on the device is of type low as defined by the Android documentation.|
|medium|2|The required password complexity on the device is of type medium as defined by the Android documentation.|
|high|3|The required password complexity on the device is of type high as defined by the Android documentation.|