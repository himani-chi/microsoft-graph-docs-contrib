---
title: "mobileAppTroubleshootingEvent resource type"
description: "MobileAppTroubleshootingEvent Entity."
author: "jaiprakashmb"
ms.localizationpriority: medium
ms.subservice: "intune"
doc_type: resourcePageType
ms.date: 08/01/2024
---

# mobileAppTroubleshootingEvent resource type

Namespace: microsoft.graph

> **Important:** APIs under the /beta version in Microsoft Graph are subject to change which could break your applications. While Intune /beta APIs are supported by Microsoft, you should use these at your own discretion. In general, /beta APIs are not recommended for use in production applications. To determine whether an API is available in v1.0, use the Version selector

> **Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.

MobileAppTroubleshootingEvent Entity.

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List mobileAppTroubleshootingEvents](../api/intune-devices-mobileapptroubleshootingevent-list.md)|[mobileAppTroubleshootingEvent](../resources/intune-devices-mobileapptroubleshootingevent.md) collection|List properties and relationships of the [mobileAppTroubleshootingEvent](../resources/intune-devices-mobileapptroubleshootingevent.md) objects.|
|[Get mobileAppTroubleshootingEvent](../api/intune-devices-mobileapptroubleshootingevent-get.md)|[mobileAppTroubleshootingEvent](../resources/intune-devices-mobileapptroubleshootingevent.md)|Read properties and relationships of the [mobileAppTroubleshootingEvent](../resources/intune-devices-mobileapptroubleshootingevent.md) object.|
|[Create mobileAppTroubleshootingEvent](../api/intune-devices-mobileapptroubleshootingevent-create.md)|[mobileAppTroubleshootingEvent](../resources/intune-devices-mobileapptroubleshootingevent.md)|Create a new [mobileAppTroubleshootingEvent](../resources/intune-devices-mobileapptroubleshootingevent.md) object.|
|[Delete mobileAppTroubleshootingEvent](../api/intune-devices-mobileapptroubleshootingevent-delete.md)|None|Deletes a [mobileAppTroubleshootingEvent](../resources/intune-devices-mobileapptroubleshootingevent.md).|
|[Update mobileAppTroubleshootingEvent](../api/intune-devices-mobileapptroubleshootingevent-update.md)|[mobileAppTroubleshootingEvent](../resources/intune-devices-mobileapptroubleshootingevent.md)|Update the properties of a [mobileAppTroubleshootingEvent](../resources/intune-devices-mobileapptroubleshootingevent.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|The GUID for the object|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|appLogCollectionRequests|[appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) collection|Indicates collection of App Log Upload Request.|

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileAppTroubleshootingEvent"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingEvent",
  "id": "String (identifier)"
}
```
