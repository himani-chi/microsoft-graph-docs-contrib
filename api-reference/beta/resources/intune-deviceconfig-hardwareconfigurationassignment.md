---
title: "hardwareConfigurationAssignment resource type"
description: "Contains properties used to assign a hardware configuration to a group."
author: "jaiprakashmb"
ms.localizationpriority: medium
ms.subservice: "intune"
doc_type: resourcePageType
ms.date: 08/01/2024
---

# hardwareConfigurationAssignment resource type

Namespace: microsoft.graph

> **Important:** APIs under the /beta version in Microsoft Graph are subject to change which could break your applications. While Intune /beta APIs are supported by Microsoft, you should use these at your own discretion. In general, /beta APIs are not recommended for use in production applications. To determine whether an API is available in v1.0, use the Version selector

> **Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.

Contains properties used to assign a hardware configuration to a group.

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List hardwareConfigurationAssignments](../api/intune-deviceconfig-hardwareconfigurationassignment-list.md)|[hardwareConfigurationAssignment](../resources/intune-deviceconfig-hardwareconfigurationassignment.md) collection|List properties and relationships of the [hardwareConfigurationAssignment](../resources/intune-deviceconfig-hardwareconfigurationassignment.md) objects.|
|[Get hardwareConfigurationAssignment](../api/intune-deviceconfig-hardwareconfigurationassignment-get.md)|[hardwareConfigurationAssignment](../resources/intune-deviceconfig-hardwareconfigurationassignment.md)|Read properties and relationships of the [hardwareConfigurationAssignment](../resources/intune-deviceconfig-hardwareconfigurationassignment.md) object.|
|[Create hardwareConfigurationAssignment](../api/intune-deviceconfig-hardwareconfigurationassignment-create.md)|[hardwareConfigurationAssignment](../resources/intune-deviceconfig-hardwareconfigurationassignment.md)|Create a new [hardwareConfigurationAssignment](../resources/intune-deviceconfig-hardwareconfigurationassignment.md) object.|
|[Delete hardwareConfigurationAssignment](../api/intune-deviceconfig-hardwareconfigurationassignment-delete.md)|None|Deletes a [hardwareConfigurationAssignment](../resources/intune-deviceconfig-hardwareconfigurationassignment.md).|
|[Update hardwareConfigurationAssignment](../api/intune-deviceconfig-hardwareconfigurationassignment-update.md)|[hardwareConfigurationAssignment](../resources/intune-deviceconfig-hardwareconfigurationassignment.md)|Update the properties of a [hardwareConfigurationAssignment](../resources/intune-deviceconfig-hardwareconfigurationassignment.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|Key of the hardware configuration group assignment entity. This property is read-only.|
|target|[deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|The Id of the Azure Active Directory group we are targeting the configuration to.|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.hardwareConfigurationAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.hardwareConfigurationAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.organizationalUnitAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "String",
    "deviceAndAppManagementAssignmentFilterType": "String",
    "organizationalUnitId": "String",
    "assignmentConflictSetting": {
      "@odata.type": "microsoft.graph.organizationalUnitAssignmentConflictSetting",
      "assignmentOverride": "String",
      "versionNumber": 1024
    }
  }
}
```