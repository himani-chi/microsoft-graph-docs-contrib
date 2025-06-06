---
title: "assignmentFilterEvaluationSummary resource type"
description: "Represent result summary for assignment filter evaluation"
author: "jaiprakashmb"
ms.localizationpriority: medium
ms.subservice: "intune"
doc_type: resourcePageType
ms.date: 08/01/2024
---

# assignmentFilterEvaluationSummary resource type

Namespace: microsoft.graph

> **Important:** APIs under the /beta version in Microsoft Graph are subject to change which could break your applications. While Intune /beta APIs are supported by Microsoft, you should use these at your own discretion. In general, /beta APIs are not recommended for use in production applications. To determine whether an API is available in v1.0, use the Version selector

> **Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.

Represent result summary for assignment filter evaluation

## Properties
|Property|Type|Description|
|:---|:---|:---|
|assignmentFilterId|String|Unique identifier for the assignment filter object|
|assignmentFilterLastModifiedDateTime|DateTimeOffset|The time the assignment filter was last modified.|
|assignmentFilterDisplayName|String|The admin defined name for assignment filter.|
|assignmentFilterPlatform|[devicePlatformType](../resources/intune-policyset-deviceplatformtype.md)|The platform for which this assignment filter is created. Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`, `androidAOSP`, `androidMobileApplicationManagement`, `iOSMobileApplicationManagement`, `unknownFutureValue`, `windowsMobileApplicationManagement`.|
|evaluationResult|[assignmentFilterEvaluationResult](../resources/intune-policyset-assignmentfilterevaluationresult.md)|Assignment filter evaluation result. Possible values are: `unknown`, `match`, `notMatch`, `inconclusive`, `failure`, `notEvaluated`.|
|evaluationDateTime|DateTimeOffset|The time assignment filter was evaluated.|
|assignmentFilterType|[deviceAndAppManagementAssignmentFilterType](../resources/intune-shared-deviceandappmanagementassignmentfiltertype.md)|Indicate filter type either include or exclude. Possible values are: `none`, `include`, `exclude`.|
|assignmentFilterTypeAndEvaluationResults|[assignmentFilterTypeAndEvaluationResult](../resources/intune-policyset-assignmentfiltertypeandevaluationresult.md) collection|A collection of filter types and their corresponding evaluation results.|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.assignmentFilterEvaluationSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.assignmentFilterEvaluationSummary",
  "assignmentFilterId": "String",
  "assignmentFilterLastModifiedDateTime": "String (timestamp)",
  "assignmentFilterDisplayName": "String",
  "assignmentFilterPlatform": "String",
  "evaluationResult": "String",
  "evaluationDateTime": "String (timestamp)",
  "assignmentFilterType": "String",
  "assignmentFilterTypeAndEvaluationResults": [
    {
      "@odata.type": "microsoft.graph.assignmentFilterTypeAndEvaluationResult",
      "assignmentFilterType": "String",
      "evaluationResult": "String"
    }
  ]
}
```