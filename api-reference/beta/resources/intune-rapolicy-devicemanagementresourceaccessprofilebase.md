---
title: "deviceManagementResourceAccessProfileBase resource type"
description: "Base Profile Type for Resource Access"
author: "jaiprakashmb"
ms.localizationpriority: medium
ms.subservice: "intune"
doc_type: resourcePageType
ms.date: 08/01/2024
---

# deviceManagementResourceAccessProfileBase resource type

Namespace: microsoft.graph

> **Important:** APIs under the /beta version in Microsoft Graph are subject to change which could break your applications. While Intune /beta APIs are supported by Microsoft, you should use these at your own discretion. In general, /beta APIs are not recommended for use in production applications. To determine whether an API is available in v1.0, use the Version selector

> **Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.

Base Profile Type for Resource Access

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List deviceManagementResourceAccessProfileBases](../api/intune-rapolicy-devicemanagementresourceaccessprofilebase-list.md)|[deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md) collection|List properties and relationships of the [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md) objects.|
|[Get deviceManagementResourceAccessProfileBase](../api/intune-rapolicy-devicemanagementresourceaccessprofilebase-get.md)|[deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)|Read properties and relationships of the [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md) object.|
|[assign action](../api/intune-rapolicy-devicemanagementresourceaccessprofilebase-assign.md)|[deviceManagementResourceAccessProfileAssignment](../resources/intune-rapolicy-devicemanagementresourceaccessprofileassignment.md) collection||
|[queryByPlatformType action](../api/intune-rapolicy-devicemanagementresourceaccessprofilebase-querybyplatformtype.md)|[deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md) collection||

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|Profile identifier|
|version|Int32|Version of the profile|
|displayName|String|Profile display name|
|description|String|Profile description|
|creationDateTime|DateTimeOffset|DateTime profile was created|
|lastModifiedDateTime|DateTimeOffset|DateTime profile was last modified|
|roleScopeTagIds|String collection|Scope Tags|
|serverApplicabilityRules|[applicabilityRule](../resources/intune-rapolicy-applicabilityrule.md) collection|The list of Applicability Rules for a Device Configuration Profile|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|assignments|[deviceManagementResourceAccessProfileAssignment](../resources/intune-rapolicy-devicemanagementresourceaccessprofileassignment.md) collection|The list of assignments for the device configuration profile.|

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementResourceAccessProfileBase"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementResourceAccessProfileBase",
  "id": "String (identifier)",
  "version": 1024,
  "displayName": "String",
  "description": "String",
  "creationDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "roleScopeTagIds": [
    "String"
  ],
  "serverApplicabilityRules": [
    {
      "@odata.type": "microsoft.graph.osVersionApplicabilityRule",
      "filterType": "String",
      "minOSVersion": "String",
      "maxOSVersion": "String"
    }
  ]
}
```