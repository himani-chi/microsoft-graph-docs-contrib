---
title: "comanagementEligibleDevicesSummary resource type"
description: "Intune Devices Comanagementeligibledevicessummary Resources ."
author: "jaiprakashmb"
ms.localizationpriority: medium
ms.subservice: "intune"
doc_type: resourcePageType
ms.date: 08/01/2024
---

# comanagementEligibleDevicesSummary resource type

Namespace: microsoft.graph

> **Important:** APIs under the /beta version in Microsoft Graph are subject to change which could break your applications. While Intune /beta APIs are supported by Microsoft, you should use these at your own discretion. In general, /beta APIs are not recommended for use in production applications. To determine whether an API is available in v1.0, use the Version selector

> **Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.



## Properties
|Property|Type|Description|
|:---|:---|:---|
|comanagedCount|Int32|Count of devices already Co-Managed|
|eligibleCount|Int32|Count of devices fully eligible for Co-Management|
|scheduledForEnrollmentCount|Int32|Count of devices scheduled for Co-Management enrollment. Valid values 0 to 9999999|
|eligibleButNotAzureAdJoinedCount|Int32|Count of devices eligible for Co-Management but not yet joined to Azure Active Directory|
|needsOsUpdateCount|Int32|Count of devices that will be eligible for Co-Management after an OS update|
|ineligibleCount|Int32|Count of devices ineligible for Co-Management|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.comanagementEligibleDevicesSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.comanagementEligibleDevicesSummary",
  "comanagedCount": 1024,
  "eligibleCount": 1024,
  "scheduledForEnrollmentCount": 1024,
  "eligibleButNotAzureAdJoinedCount": 1024,
  "needsOsUpdateCount": 1024,
  "ineligibleCount": 1024
}
```