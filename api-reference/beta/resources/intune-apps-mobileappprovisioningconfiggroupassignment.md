---
title: "mobileAppProvisioningConfigGroupAssignment resource type"
description: "Contains the properties used to assign an App provisioning configuration to a group."
author: "jaiprakashmb"
ms.localizationpriority: medium
ms.subservice: "intune"
doc_type: resourcePageType
ms.date: 08/01/2024
---

# mobileAppProvisioningConfigGroupAssignment resource type

Namespace: microsoft.graph

> **Important:** APIs under the /beta version in Microsoft Graph are subject to change which could break your applications. While Intune /beta APIs are supported by Microsoft, you should use these at your own discretion. In general, /beta APIs are not recommended for use in production applications. To determine whether an API is available in v1.0, use the Version selector

> **Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.

Contains the properties used to assign an App provisioning configuration to a group.

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List mobileAppProvisioningConfigGroupAssignments](../api/intune-apps-mobileappprovisioningconfiggroupassignment-list.md)|[mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) collection|List properties and relationships of the [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) objects.|
|[Get mobileAppProvisioningConfigGroupAssignment](../api/intune-apps-mobileappprovisioningconfiggroupassignment-get.md)|[mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)|Read properties and relationships of the [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) object.|
|[Create mobileAppProvisioningConfigGroupAssignment](../api/intune-apps-mobileappprovisioningconfiggroupassignment-create.md)|[mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)|Create a new [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) object.|
|[Delete mobileAppProvisioningConfigGroupAssignment](../api/intune-apps-mobileappprovisioningconfiggroupassignment-delete.md)|None|Deletes a [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md).|
|[Update mobileAppProvisioningConfigGroupAssignment](../api/intune-apps-mobileappprovisioningconfiggroupassignment-update.md)|[mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)|Update the properties of a [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|targetGroupId|String|The ID of the AAD group in which the app provisioning configuration is being targeted.|
|id|String|Key of the entity.|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileAppProvisioningConfigGroupAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppProvisioningConfigGroupAssignment",
  "targetGroupId": "String",
  "id": "String (identifier)"
}
```