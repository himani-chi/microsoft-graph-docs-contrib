---
title: "mobileAppInstallTimeSettings resource type"
description: "Contains properties used to determine when to offer an app to devices and when to install the app on devices."
author: "jaiprakashmb"
ms.localizationpriority: medium
ms.subservice: "intune"
doc_type: resourcePageType
ms.date: 08/01/2024
---

# mobileAppInstallTimeSettings resource type

Namespace: microsoft.graph
> **Important:** APIs under the /beta version in Microsoft Graph are subject to change which could break your applications. While Intune /beta APIs are supported by Microsoft, you should use these at your own discretion. In general, /beta APIs are not recommended for use in production applications. To determine whether an API is available in v1.0, use the Version selector.

> **Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.


Contains properties used to determine when to offer an app to devices and when to install the app on devices.

## Properties
|Property|Type|Description|
|:---|:---|:---|
|useLocalTime|Boolean|Whether the local device time or UTC time should be used when determining the available and deadline times.|
|startDateTime|DateTimeOffset|The time at which the app should be available for installation.|
|deadlineDateTime|DateTimeOffset|The time at which the app should be installed.|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mobileAppInstallTimeSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppInstallTimeSettings",
  "useLocalTime": true,
  "startDateTime": "String (timestamp)",
  "deadlineDateTime": "String (timestamp)"
}
```
