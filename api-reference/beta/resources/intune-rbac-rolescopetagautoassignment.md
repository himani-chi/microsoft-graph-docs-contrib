---
title: "roleScopeTagAutoAssignment resource type"
description: "Contains the properties for auto-assigning a Role Scope Tag to a group to be applied to Devices."
author: "jaiprakashmb"
ms.localizationpriority: medium
ms.subservice: "intune"
doc_type: resourcePageType
ms.date: 08/01/2024
---

# roleScopeTagAutoAssignment resource type

Namespace: microsoft.graph

> **Important:** APIs under the /beta version in Microsoft Graph are subject to change which could break your applications. While Intune /beta APIs are supported by Microsoft, you should use these at your own discretion. In general, /beta APIs are not recommended for use in production applications. To determine whether an API is available in v1.0, use the Version selector

> **Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.

Contains the properties for auto-assigning a Role Scope Tag to a group to be applied to Devices.

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List roleScopeTagAutoAssignments](../api/intune-rbac-rolescopetagautoassignment-list.md)|[roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) collection|List properties and relationships of the [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) objects.|
|[Get roleScopeTagAutoAssignment](../api/intune-rbac-rolescopetagautoassignment-get.md)|[roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md)|Read properties and relationships of the [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) object.|
|[Create roleScopeTagAutoAssignment](../api/intune-rbac-rolescopetagautoassignment-create.md)|[roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md)|Create a new [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) object.|
|[Delete roleScopeTagAutoAssignment](../api/intune-rbac-rolescopetagautoassignment-delete.md)|None|Deletes a [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md).|
|[Update roleScopeTagAutoAssignment](../api/intune-rbac-rolescopetagautoassignment-update.md)|[roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md)|Update the properties of a [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|Key of the entity. This property is read-only.|
|target|[deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|The auto-assignment target for the specific Role Scope Tag.|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.roleScopeTagAutoAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.roleScopeTagAutoAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.scopeTagGroupAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "String",
    "deviceAndAppManagementAssignmentFilterType": "String",
    "targetType": "String",
    "entraObjectId": "String"
  }
}
```