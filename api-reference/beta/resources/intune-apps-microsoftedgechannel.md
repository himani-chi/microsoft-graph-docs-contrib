---
title: "microsoftEdgeChannel enum type"
description: "The enum to specify the channels for Microsoft Edge apps."
author: "jaiprakashmb"
ms.localizationpriority: medium
ms.subservice: "intune"
doc_type: enumPageType
ms.date: 08/01/2024
---

# microsoftEdgeChannel enum type

Namespace: microsoft.graph

> **Important:** APIs under the /beta version in Microsoft Graph are subject to change which could break your applications. While Intune /beta APIs are supported by Microsoft, you should use these at your own discretion. In general, /beta APIs are not recommended for use in production applications. To determine whether an API is available in v1.0, use the Version selector

> **Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.

The enum to specify the channels for Microsoft Edge apps.

## Members
|Member|Value|Description|
|:---|:---|:---|
|dev|0|The Dev Channel is intended to help you plan and develop with the latest capabilities of Microsoft Edge.|
|beta|1|The Beta Channel is intended for production deployment to a representative sample set of users. New features ship about every 4 weeks. Security and quality updates ship as needed.|
|stable|2|The Stable Channel is intended for broad deployment within organizations, and it's the channel that most users should be on. New features ship about every 4 weeks. Security and quality updates ship as needed.|
|unknownFutureValue|3|Evolvable enumeration sentinel value. Do not use.|