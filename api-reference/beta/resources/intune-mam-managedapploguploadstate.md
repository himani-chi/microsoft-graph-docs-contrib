---
title: "managedAppLogUploadState enum type"
description: "Represents the current status of the associated `managedAppLogCollectionRequest`."
author: "jaiprakashmb"
ms.localizationpriority: medium
ms.subservice: "intune"
doc_type: enumPageType
ms.date: 08/01/2024
---

# managedAppLogUploadState enum type

Namespace: microsoft.graph

> **Important:** APIs under the /beta version in Microsoft Graph are subject to change which could break your applications. While Intune /beta APIs are supported by Microsoft, you should use these at your own discretion. In general, /beta APIs are not recommended for use in production applications. To determine whether an API is available in v1.0, use the Version selector

> **Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.

Represents the current status of the associated `managedAppLogCollectionRequest`.

## Members
|Member|Value|Description|
|:---|:---|:---|
|pending|0|Default. The log upload request has been successfully created, and is pending delivery to the Mobile Application Management (MAM) application.|
|inProgress|1|One or more log upload components have uploaded their logs.|
|completed|2|All log upload successfully components have uploaded their logs.|
|declinedByUser|3|The log upload request was declined by the user on the device.|
|timedOut|4|The log upload request was not acknowledged by the user within the allowed time window.|
|failed|5|The log upload request encountered an error.|
|unknownFutureValue|6|Evolvable enumeration sentinel value. Do not use.|