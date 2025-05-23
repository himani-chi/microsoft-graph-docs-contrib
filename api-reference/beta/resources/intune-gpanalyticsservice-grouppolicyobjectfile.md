---
title: "groupPolicyObjectFile resource type"
description: "The Group Policy Object file uploaded by admin."
author: "jaiprakashmb"
ms.localizationpriority: medium
ms.subservice: "intune"
doc_type: resourcePageType
ms.date: 08/01/2024
---

# groupPolicyObjectFile resource type

Namespace: microsoft.graph

> **Important:** APIs under the /beta version in Microsoft Graph are subject to change which could break your applications. While Intune /beta APIs are supported by Microsoft, you should use these at your own discretion. In general, /beta APIs are not recommended for use in production applications. To determine whether an API is available in v1.0, use the Version selector

> **Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.

The Group Policy Object file uploaded by admin.

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List groupPolicyObjectFiles](../api/intune-gpanalyticsservice-grouppolicyobjectfile-list.md)|[groupPolicyObjectFile](../resources/intune-gpanalyticsservice-grouppolicyobjectfile.md) collection|List properties and relationships of the [groupPolicyObjectFile](../resources/intune-gpanalyticsservice-grouppolicyobjectfile.md) objects.|
|[Get groupPolicyObjectFile](../api/intune-gpanalyticsservice-grouppolicyobjectfile-get.md)|[groupPolicyObjectFile](../resources/intune-gpanalyticsservice-grouppolicyobjectfile.md)|Read properties and relationships of the [groupPolicyObjectFile](../resources/intune-gpanalyticsservice-grouppolicyobjectfile.md) object.|
|[Create groupPolicyObjectFile](../api/intune-gpanalyticsservice-grouppolicyobjectfile-create.md)|[groupPolicyObjectFile](../resources/intune-gpanalyticsservice-grouppolicyobjectfile.md)|Create a new [groupPolicyObjectFile](../resources/intune-gpanalyticsservice-grouppolicyobjectfile.md) object.|
|[Delete groupPolicyObjectFile](../api/intune-gpanalyticsservice-grouppolicyobjectfile-delete.md)|None|Deletes a [groupPolicyObjectFile](../resources/intune-gpanalyticsservice-grouppolicyobjectfile.md).|
|[Update groupPolicyObjectFile](../api/intune-gpanalyticsservice-grouppolicyobjectfile-update.md)|[groupPolicyObjectFile](../resources/intune-gpanalyticsservice-grouppolicyobjectfile.md)|Update the properties of a [groupPolicyObjectFile](../resources/intune-gpanalyticsservice-grouppolicyobjectfile.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String||
|groupPolicyObjectId|Guid|The Group Policy Object GUID from GPO Xml content|
|ouDistinguishedName|String|The distinguished name of the OU.|
|createdDateTime|DateTimeOffset|The date and time at which the GroupPolicy was first uploaded.|
|lastModifiedDateTime|DateTimeOffset|The date and time at which the GroupPolicyObjectFile was last modified.|
|content|String|The Group Policy Object file content.|
|roleScopeTagIds|String collection|The list of scope tags for the configuration.|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyObjectFile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyObjectFile",
  "id": "String (identifier)",
  "groupPolicyObjectId": "Guid",
  "ouDistinguishedName": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "content": "String",
  "roleScopeTagIds": [
    "String"
  ]
}
```