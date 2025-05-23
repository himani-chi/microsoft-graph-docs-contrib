---
title: "userExperienceAnalyticsDeviceStatus enum type"
description: "Indicates the status of the device in the correlation group. Eg: Device status can be anomalous, affected, at risk."
author: "jaiprakashmb"
ms.localizationpriority: medium
ms.subservice: "intune"
doc_type: enumPageType
ms.date: 08/01/2024
---

# userExperienceAnalyticsDeviceStatus enum type

Namespace: microsoft.graph

> **Important:** APIs under the /beta version in Microsoft Graph are subject to change which could break your applications. While Intune /beta APIs are supported by Microsoft, you should use these at your own discretion. In general, /beta APIs are not recommended for use in production applications. To determine whether an API is available in v1.0, use the Version selector

> **Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.

Indicates the status of the device in the correlation group. Eg: Device status can be anomalous, affected, at risk.

## Members
|Member|Value|Description|
|:---|:---|:---|
|anomalous|0|Indicates the the device is part of the anomaly.|
|affected|1|Indicates the device is affected by the anomaly and is part of the correlation group.|
|atRisk|2|Indicates the device is not part of the anomaly but is part of the correlation group.|
|unknownFutureValue|3|Evolvable enumeration sentinel value. Do not use.|