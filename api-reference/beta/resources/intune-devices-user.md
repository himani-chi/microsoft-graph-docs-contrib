---
title: "user resource type"
description: "Intune Devices User Source_Resources ."
author: "jaiprakashmb"
ms.localizationpriority: medium
ms.subservice: "intune"
doc_type: resourcePageType
ms.date: 09/12/2024
---

# user resource type

Namespace: microsoft.graph

> **Important:** APIs under the /beta version in Microsoft Graph are subject to change which could break your applications. While Intune /beta APIs are supported by Microsoft, you should use these at your own discretion. In general, /beta APIs are not recommended for use in production applications. To determine whether an API is available in v1.0, use the Version selector.

> **Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.



## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List users](../api/intune-devices-user-list.md)|[user](../resources/intune-devices-user.md) collection|List properties and relationships of the [user](../resources/intune-devices-user.md) objects.|
|[Get user](../api/intune-devices-user-get.md)|[user](../resources/intune-devices-user.md)|Read properties and relationships of the [user](../resources/intune-devices-user.md) object.|
|[Create user](../api/intune-devices-user-create.md)|[user](../resources/intune-devices-user.md)|Create a new [user](../resources/intune-devices-user.md) object.|
|[Delete user](../api/intune-devices-user-delete.md)|None|Deletes a [user](../resources/intune-devices-user.md).|
|[Update user](../api/intune-devices-user-update.md)|[user](../resources/intune-devices-user.md)|Update the properties of a [user](../resources/intune-devices-user.md) object.|
|[removeAllDevicesFromManagement action](../api/intune-devices-user-removealldevicesfrommanagement.md)|None|Retire all devices from management for this user|
|[getLoggedOnManagedDevices function](../api/intune-devices-user-getloggedonmanageddevices.md)|[managedDevice](../resources/intune-devices-manageddevice.md) collection||

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|Unique identifier of the user.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|managedDevices|[managedDevice](../resources/intune-devices-manageddevice.md) collection|The managed devices associated with the user.|

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.user"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.user",
  "id": "String (identifier)"
}
```
