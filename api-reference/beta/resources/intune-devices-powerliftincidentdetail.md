---
title: "powerliftIncidentDetail resource type"
description: "This type contains specific information regarding a Powerlift incident, such as when it was uploaded, the platform the device was on, and a string array of files associated to the incident."
author: "jaiprakashmb"
ms.localizationpriority: medium
ms.subservice: "intune"
doc_type: resourcePageType
ms.date: 08/01/2024
---

# powerliftIncidentDetail resource type

Namespace: microsoft.graph

> **Important:** APIs under the /beta version in Microsoft Graph are subject to change which could break your applications. While Intune /beta APIs are supported by Microsoft, you should use these at your own discretion. In general, /beta APIs are not recommended for use in production applications. To determine whether an API is available in v1.0, use the Version selector

> **Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.

This type contains specific information regarding a Powerlift incident, such as when it was uploaded, the platform the device was on, and a string array of files associated to the incident.

## Properties
|Property|Type|Description|
|:---|:---|:---|
|powerliftId|String|The unique identifier of the app diagnostic. This id is assigned to a diagnostic when it is uploaded to Powerlift. Example: 8520467a-49a9-44a4-8447-8dfb8bec6726|
|easyId|String|The unique app diagnostic identifier as a user friendly 8 character hexadecimal string. This id is smaller compared to the powerliftId. Th Example: 8520467A|
|createdDateTime|DateTimeOffset|The time the app diagnostic was created. The value cannot be modified and is automatically populated when the diagnostic is uploaded. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.Example: 2022-04-19T17:24:45.313Z|
|platformDisplayName|String|The operating system of the device from which diagnostics are collected. Example: iOS|
|applicationName|String|TThe name of the application for which the diagnostic is collected. Example: com.microsoft.CompanyPortal | No|
|clientApplicationVersion|String|The version of the application for which the diagnostic is collected. Example: 5.2203.1|
|locale|String|The locale information of the application for which the diagnostic is collected. Example: en-US|
|fileNames|String collection|A list of files that are associated with the diagnostic.|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.powerliftIncidentDetail"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.powerliftIncidentDetail",
  "powerliftId": "String",
  "easyId": "String",
  "createdDateTime": "String (timestamp)",
  "platformDisplayName": "String",
  "applicationName": "String",
  "clientApplicationVersion": "String",
  "locale": "String",
  "fileNames": [
    "String"
  ]
}
```