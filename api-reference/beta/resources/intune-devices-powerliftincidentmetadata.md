---
title: "powerliftIncidentMetadata resource type"
description: "Collection of app diagnostics associated with a user."
author: "jaiprakashmb"
ms.localizationpriority: medium
ms.subservice: "intune"
doc_type: resourcePageType
ms.date: 08/01/2024
---

# powerliftIncidentMetadata resource type

Namespace: microsoft.graph

> **Important:** APIs under the /beta version in Microsoft Graph are subject to change which could break your applications. While Intune /beta APIs are supported by Microsoft, you should use these at your own discretion. In general, /beta APIs are not recommended for use in production applications. To determine whether an API is available in v1.0, use the Version selector

> **Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.

Collection of app diagnostics associated with a user.

## Properties
|Property|Type|Description|
|:---|:---|:---|
|powerliftId|Guid|The unique identifier of the app diagnostic. Example: 8520467a-49a9-44a4-8447-8dfb8bec6726|
|easyId|String|The unique app diagnostic identifier as a user friendly 8 character hexadecimal string. Example: 8520467A|
|createdAtDateTime|DateTimeOffset|The time the app diagnostic was created. Example: 2022-04-19T17:24:45.313Z|
|platform|String|The device's OS the diagnostic is from. Example: iOS|
|application|String|The name of the application the diagnostic is from. Example: com.microsoft.CompanyPortal|
|clientVersion|String|The version of the application. Example: 5.2203.1|
|locale|String|The locale information of the application. Example: en-US|
|fileNames|String collection|A list of files that are associated with the diagnostic.|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.powerliftIncidentMetadata"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.powerliftIncidentMetadata",
  "powerliftId": "Guid",
  "easyId": "String",
  "createdAtDateTime": "String (timestamp)",
  "platform": "String",
  "application": "String",
  "clientVersion": "String",
  "locale": "String",
  "fileNames": [
    "String"
  ]
}
```