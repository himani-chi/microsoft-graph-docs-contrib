---
title: "deviceManagementResourceAccessProfileAssignment resource type"
description: "Entity that describes tenant level settings for derived credentials"
author: "jaiprakashmb"
ms.localizationpriority: medium
ms.subservice: "intune"
doc_type: resourcePageType
ms.date: 08/01/2024
---

# deviceManagementResourceAccessProfileAssignment resource type

Namespace: microsoft.graph

> **Important:** APIs under the /beta version in Microsoft Graph are subject to change which could break your applications. While Intune /beta APIs are supported by Microsoft, you should use these at your own discretion. In general, /beta APIs are not recommended for use in production applications. To determine whether an API is available in v1.0, use the Version selector

> **Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.

Entity that describes tenant level settings for derived credentials

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List deviceManagementResourceAccessProfileAssignments](../api/intune-rapolicy-devicemanagementresourceaccessprofileassignment-list.md)|[deviceManagementResourceAccessProfileAssignment](../resources/intune-rapolicy-devicemanagementresourceaccessprofileassignment.md) collection|List properties and relationships of the [deviceManagementResourceAccessProfileAssignment](../resources/intune-rapolicy-devicemanagementresourceaccessprofileassignment.md) objects.|
|[Get deviceManagementResourceAccessProfileAssignment](../api/intune-rapolicy-devicemanagementresourceaccessprofileassignment-get.md)|[deviceManagementResourceAccessProfileAssignment](../resources/intune-rapolicy-devicemanagementresourceaccessprofileassignment.md)|Read properties and relationships of the [deviceManagementResourceAccessProfileAssignment](../resources/intune-rapolicy-devicemanagementresourceaccessprofileassignment.md) object.|
|[Create deviceManagementResourceAccessProfileAssignment](../api/intune-rapolicy-devicemanagementresourceaccessprofileassignment-create.md)|[deviceManagementResourceAccessProfileAssignment](../resources/intune-rapolicy-devicemanagementresourceaccessprofileassignment.md)|Create a new [deviceManagementResourceAccessProfileAssignment](../resources/intune-rapolicy-devicemanagementresourceaccessprofileassignment.md) object.|
|[Delete deviceManagementResourceAccessProfileAssignment](../api/intune-rapolicy-devicemanagementresourceaccessprofileassignment-delete.md)|None|Deletes a [deviceManagementResourceAccessProfileAssignment](../resources/intune-rapolicy-devicemanagementresourceaccessprofileassignment.md).|
|[Update deviceManagementResourceAccessProfileAssignment](../api/intune-rapolicy-devicemanagementresourceaccessprofileassignment-update.md)|[deviceManagementResourceAccessProfileAssignment](../resources/intune-rapolicy-devicemanagementresourceaccessprofileassignment.md)|Update the properties of a [deviceManagementResourceAccessProfileAssignment](../resources/intune-rapolicy-devicemanagementresourceaccessprofileassignment.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|Unique identifier for the Assignments|
|intent|[deviceManagementResourceAccessProfileIntent](../resources/intune-rapolicy-devicemanagementresourceaccessprofileintent.md)|The assignment intent for the resource access profile. Possible values are: `apply`, `remove`.|
|target|[deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|The assignment target for the resource access profile.|
|sourceId|String|The identifier of the source of the assignment.|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementResourceAccessProfileAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementResourceAccessProfileAssignment",
  "id": "String (identifier)",
  "intent": "String",
  "target": {
    "@odata.type": "microsoft.graph.scopeTagGroupAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "String",
    "deviceAndAppManagementAssignmentFilterType": "String",
    "targetType": "String",
    "entraObjectId": "String"
  },
  "sourceId": "String"
}
```