---
title: "managementFeatureProjectDetail resource type"
description: "Intune Deviceconfig Managementfeatureprojectdetail Resources ."
author: "jaiprakashmb"
ms.localizationpriority: medium
ms.subservice: "intune"
doc_type: resourcePageType
ms.date: 10/15/2024
---

# managementFeatureProjectDetail resource type

Namespace: microsoft.graph

> **Important:** APIs under the /beta version in Microsoft Graph are subject to change which could break your applications. While Intune /beta APIs are supported by Microsoft, you should use these at your own discretion. In general, /beta APIs are not recommended for use in production applications. To determine whether an API is available in v1.0, use the Version selector.

> **Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.



## Properties
|Property|Type|Description|
|:---|:---|:---|
|projectName|String|Flighting V2 project name|
|featureFlights|[managementFeatureFlightDetail](../resources/intune-deviceconfig-managementfeatureflightdetail.md) collection|List containing feature flighting details in the project|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managementFeatureProjectDetail"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managementFeatureProjectDetail",
  "projectName": "String",
  "featureFlights": [
    {
      "@odata.type": "microsoft.graph.managementFeatureFlightDetail",
      "flightId": "String",
      "flightValue": "String"
    }
  ]
}
```
