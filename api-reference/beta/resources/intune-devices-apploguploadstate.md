---
title: "appLogUploadState enum type"
description: "AppLogUploadStatus"
author: "jaiprakashmb"
ms.localizationpriority: medium
ms.subservice: "intune"
doc_type: enumPageType
ms.date: 08/01/2024
---

# appLogUploadState enum type

Namespace: microsoft.graph

> **Important:** APIs under the /beta version in Microsoft Graph are subject to change which could break your applications. While Intune /beta APIs are supported by Microsoft, you should use these at your own discretion. In general, /beta APIs are not recommended for use in production applications. To determine whether an API is available in v1.0, use the Version selector

> **Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.

AppLogUploadStatus

## Members
|Member|Value|Description|
|:---|:---|:---|
|pending|0|Default. Indicates that request is waiting to be processed or under processing.|
|completed|1|Indicates that request is completed with file uploaded to Azure blob for download.|
|failed|2|Indicates that request is completed with file uploaded to Azure blob for download.|
|unknownFutureValue|3|Evolvable enumeration sentinel value. Do not use.|