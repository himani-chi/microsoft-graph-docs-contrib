---
title: "deviceManagementBooleanSettingInstance resource type"
description: "A setting instance representing a boolean value"
author: "jaiprakashmb"
ms.localizationpriority: medium
ms.subservice: "intune"
doc_type: resourcePageType
ms.date: 08/01/2024
---

# deviceManagementBooleanSettingInstance resource type

Namespace: microsoft.graph

> **Important:** APIs under the /beta version in Microsoft Graph are subject to change which could break your applications. While Intune /beta APIs are supported by Microsoft, you should use these at your own discretion. In general, /beta APIs are not recommended for use in production applications. To determine whether an API is available in v1.0, use the Version selector

> **Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.

A setting instance representing a boolean value


Inherits from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List deviceManagementBooleanSettingInstances](../api/intune-deviceintent-devicemanagementbooleansettinginstance-list.md)|[deviceManagementBooleanSettingInstance](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md) collection|List properties and relationships of the [deviceManagementBooleanSettingInstance](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md) objects.|
|[Get deviceManagementBooleanSettingInstance](../api/intune-deviceintent-devicemanagementbooleansettinginstance-get.md)|[deviceManagementBooleanSettingInstance](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md)|Read properties and relationships of the [deviceManagementBooleanSettingInstance](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md) object.|
|[Create deviceManagementBooleanSettingInstance](../api/intune-deviceintent-devicemanagementbooleansettinginstance-create.md)|[deviceManagementBooleanSettingInstance](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md)|Create a new [deviceManagementBooleanSettingInstance](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md) object.|
|[Delete deviceManagementBooleanSettingInstance](../api/intune-deviceintent-devicemanagementbooleansettinginstance-delete.md)|None|Deletes a [deviceManagementBooleanSettingInstance](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md).|
|[Update deviceManagementBooleanSettingInstance](../api/intune-deviceintent-devicemanagementbooleansettinginstance-update.md)|[deviceManagementBooleanSettingInstance](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md)|Update the properties of a [deviceManagementBooleanSettingInstance](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|The setting instance ID Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)|
|definitionId|String|The ID of the setting definition for this instance Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)|
|valueJson|String|JSON representation of the value Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)|
|value|Boolean|The boolean value|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementBooleanSettingInstance"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementBooleanSettingInstance",
  "id": "String (identifier)",
  "definitionId": "String",
  "valueJson": "String",
  "value": true
}
```