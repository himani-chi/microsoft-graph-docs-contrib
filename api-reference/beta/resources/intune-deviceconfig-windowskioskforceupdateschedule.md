---
title: "windowsKioskForceUpdateSchedule resource type"
description: "Windows 10 force update schedule for Kiosk devices."
author: "jaiprakashmb"
ms.localizationpriority: medium
ms.subservice: "intune"
doc_type: resourcePageType
ms.date: 08/01/2024
---

# windowsKioskForceUpdateSchedule resource type

Namespace: microsoft.graph

> **Important:** APIs under the /beta version in Microsoft Graph are subject to change which could break your applications. While Intune /beta APIs are supported by Microsoft, you should use these at your own discretion. In general, /beta APIs are not recommended for use in production applications. To determine whether an API is available in v1.0, use the Version selector

> **Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.

Windows 10 force update schedule for Kiosk devices.

## Properties
|Property|Type|Description|
|:---|:---|:---|
|startDateTime|DateTimeOffset|The start time for the force restart.|
|recurrence|[windows10AppsUpdateRecurrence](../resources/intune-deviceconfig-windows10appsupdaterecurrence.md)|Recurrence schedule. Possible values are: `none`, `daily`, `weekly`, `monthly`.|
|dayofWeek|[dayOfWeek](../resources/intune-deviceconfig-dayofweek.md)|Day of week. Possible values are: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.|
|dayofMonth|Int32|Day of month. Valid values 1 to 31|
|runImmediatelyIfAfterStartDateTime|Boolean|If true, runs the task immediately if StartDateTime is in the past, else, runs at the next recurrence.|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskForceUpdateSchedule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskForceUpdateSchedule",
  "startDateTime": "String (timestamp)",
  "recurrence": "String",
  "dayofWeek": "String",
  "dayofMonth": 1024,
  "runImmediatelyIfAfterStartDateTime": true
}
```