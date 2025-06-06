---
title: "subjectNameFormat enum type"
description: "Subject Name Format Options."
author: "jaiprakashmb"
ms.localizationpriority: medium
ms.subservice: "intune"
doc_type: enumPageType
ms.date: 08/01/2024
---

# subjectNameFormat enum type

Namespace: microsoft.graph

> **Important:** APIs under the /beta version in Microsoft Graph are subject to change which could break your applications. While Intune /beta APIs are supported by Microsoft, you should use these at your own discretion. In general, /beta APIs are not recommended for use in production applications. To determine whether an API is available in v1.0, use the Version selector

> **Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.

Subject Name Format Options.

## Members
|Member|Value|Description|
|:---|:---|:---|
|commonName|0|Common name.|
|commonNameIncludingEmail|1|Common Name Including Email.|
|commonNameAsEmail|2|Common Name As Email.|
|custom|3|Custom subject name format.|
|commonNameAsIMEI|5|Common Name As IMEI.|
|commonNameAsSerialNumber|6|Common Name As Serial Number.|
|commonNameAsAadDeviceId|7|Common Name As Serial Number.|
|commonNameAsIntuneDeviceId|8|Common Name As Serial Number.|
|commonNameAsDurableDeviceId|9|Common Name As Serial Number.|