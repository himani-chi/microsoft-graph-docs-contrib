---
title: "windowsQualityUpdatePolicyAssignment resource type"
description: "This entity contains the properties used to assign a Windows quality update policy to a group."
author: "jaiprakashmb"
ms.localizationpriority: medium
ms.subservice: "intune"
doc_type: resourcePageType
ms.date: 08/01/2024
---

# windowsQualityUpdatePolicyAssignment resource type

Namespace: microsoft.graph

> **Important:** APIs under the /beta version in Microsoft Graph are subject to change which could break your applications. While Intune /beta APIs are supported by Microsoft, you should use these at your own discretion. In general, /beta APIs are not recommended for use in production applications. To determine whether an API is available in v1.0, use the Version selector

> **Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.

This entity contains the properties used to assign a Windows quality update policy to a group.

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List windowsQualityUpdatePolicyAssignments](../api/intune-softwareupdate-windowsqualityupdatepolicyassignment-list.md)|[windowsQualityUpdatePolicyAssignment](../resources/intune-softwareupdate-windowsqualityupdatepolicyassignment.md) collection|List properties and relationships of the [windowsQualityUpdatePolicyAssignment](../resources/intune-softwareupdate-windowsqualityupdatepolicyassignment.md) objects.|
|[Get windowsQualityUpdatePolicyAssignment](../api/intune-softwareupdate-windowsqualityupdatepolicyassignment-get.md)|[windowsQualityUpdatePolicyAssignment](../resources/intune-softwareupdate-windowsqualityupdatepolicyassignment.md)|Read properties and relationships of the [windowsQualityUpdatePolicyAssignment](../resources/intune-softwareupdate-windowsqualityupdatepolicyassignment.md) object.|
|[Create windowsQualityUpdatePolicyAssignment](../api/intune-softwareupdate-windowsqualityupdatepolicyassignment-create.md)|[windowsQualityUpdatePolicyAssignment](../resources/intune-softwareupdate-windowsqualityupdatepolicyassignment.md)|Create a new [windowsQualityUpdatePolicyAssignment](../resources/intune-softwareupdate-windowsqualityupdatepolicyassignment.md) object.|
|[Delete windowsQualityUpdatePolicyAssignment](../api/intune-softwareupdate-windowsqualityupdatepolicyassignment-delete.md)|None|Deletes a [windowsQualityUpdatePolicyAssignment](../resources/intune-softwareupdate-windowsqualityupdatepolicyassignment.md).|
|[Update windowsQualityUpdatePolicyAssignment](../api/intune-softwareupdate-windowsqualityupdatepolicyassignment-update.md)|[windowsQualityUpdatePolicyAssignment](../resources/intune-softwareupdate-windowsqualityupdatepolicyassignment.md)|Update the properties of a [windowsQualityUpdatePolicyAssignment](../resources/intune-softwareupdate-windowsqualityupdatepolicyassignment.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|The id for CloudQualityUpdateProfileAssignment entity. This id is assigned when assigning the profile to a group. Read-only|
|target|[deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|The assignment target that the Windows quality update policy is assigned to.|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsQualityUpdatePolicyAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsQualityUpdatePolicyAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "String",
    "deviceAndAppManagementAssignmentFilterType": "String"
  }
}
```