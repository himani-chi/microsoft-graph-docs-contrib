---
title: "organizationalUnitAssignmentConflictSetting resource type"
description: "Represents conflict settings for an Organizational Unit (OU) payload assignment. Conflict settings are used to resolve relative priority of assigned payloads within an OU's conflict area. This helps in resolving conflicts when a same device/user setting is updated by different payloads. The payload with the lower rank takes precedence."
author: "jaiprakashmb"
ms.localizationpriority: medium
ms.subservice: "intune"
doc_type: resourcePageType
ms.date: 08/01/2024
---

# organizationalUnitAssignmentConflictSetting resource type

Namespace: microsoft.graph

> **Important:** APIs under the /beta version in Microsoft Graph are subject to change which could break your applications. While Intune /beta APIs are supported by Microsoft, you should use these at your own discretion. In general, /beta APIs are not recommended for use in production applications. To determine whether an API is available in v1.0, use the Version selector

> **Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.

Represents conflict settings for an Organizational Unit (OU) payload assignment. Conflict settings are used to resolve relative priority of assigned payloads within an OU's conflict area. This helps in resolving conflicts when a same device/user setting is updated by different payloads. The payload with the lower rank takes precedence.

## Properties
|Property|Type|Description|
|:---|:---|:---|
|assignmentOverride|[organizationalUnitAssignmentOverride](../resources/intune-shared-organizationalunitassignmentoverride.md)|Default is allowed. Indicates if a payload assignment can override the inherited assignments from ancestors in an Organizational Unit (OU) lineage. Possible values are allowed and denied. At a particular hierarchy depth, relative rank order is evaluated first to determine the winner. The override setting is used only to resolve conflicts between ancestors and descendants in a hierarchy. For example, consider a hierarchy with OU1 and OU2, where OU1 is the parent of OU2. If both OU1 and OU2 have allowed, the payload assigned to OU2 can override the payload assigned to OU1. However, if either OU1 or OU2 has denied, the payload assigned to OU1 will override the payload assigned to OU2. Possible values are: `allowed`, `denied`, `unknown`, `unknownFutureValue`.|
|versionNumber|Int32|Indicates the version of the ConflictSetting. It is updated whenever a conflict setting is modified. Valid values 0 to 5000|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.organizationalUnitAssignmentConflictSetting"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.organizationalUnitAssignmentConflictSetting",
  "assignmentOverride": "String",
  "versionNumber": 1024
}
```