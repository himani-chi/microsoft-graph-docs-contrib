---
title: "iosVppAppAssignedLicense resource type"
description: "iOS Volume Purchase Program license assignment. This class does not support Create, Delete, or Update."
author: "jaiprakashmb"
ms.localizationpriority: medium
ms.subservice: "intune"
doc_type: resourcePageType
ms.date: 08/01/2024
---

# iosVppAppAssignedLicense resource type

Namespace: microsoft.graph

> **Important:** APIs under the /beta version in Microsoft Graph are subject to change which could break your applications. While Intune /beta APIs are supported by Microsoft, you should use these at your own discretion. In general, /beta APIs are not recommended for use in production applications. To determine whether an API is available in v1.0, use the Version selector

> **Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.

iOS Volume Purchase Program license assignment. This class does not support Create, Delete, or Update.

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List iosVppAppAssignedLicenses](../api/intune-apps-iosvppappassignedlicense-list.md)|[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) collection|List properties and relationships of the [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) objects.|
|[Get iosVppAppAssignedLicense](../api/intune-apps-iosvppappassignedlicense-get.md)|[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)|Read properties and relationships of the [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) object.|
|[Create iosVppAppAssignedLicense](../api/intune-apps-iosvppappassignedlicense-create.md)|[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)|Create a new [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) object.|
|[Delete iosVppAppAssignedLicense](../api/intune-apps-iosvppappassignedlicense-delete.md)|None|Deletes a [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md).|
|[Update iosVppAppAssignedLicense](../api/intune-apps-iosvppappassignedlicense-update.md)|[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)|Update the properties of a [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|Key of the entity. This property is read-only.|
|userEmailAddress|String|The user email address.|
|userId|String|The user ID.|
|userName|String|The user name.|
|userPrincipalName|String|The user principal name.|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosVppAppAssignedLicense"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosVppAppAssignedLicense",
  "id": "String (identifier)",
  "userEmailAddress": "String",
  "userId": "String",
  "userName": "String",
  "userPrincipalName": "String"
}
```