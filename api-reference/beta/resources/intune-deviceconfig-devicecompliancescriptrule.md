---
title: "deviceComplianceScriptRule resource type"
description: "Intune Deviceconfig Devicecompliancescriptrule Resources ."
author: "jaiprakashmb"
ms.localizationpriority: medium
ms.subservice: "intune"
doc_type: resourcePageType
ms.date: 08/01/2024
---

# deviceComplianceScriptRule resource type

Namespace: microsoft.graph

> **Important:** APIs under the /beta version in Microsoft Graph are subject to change which could break your applications. While Intune /beta APIs are supported by Microsoft, you should use these at your own discretion. In general, /beta APIs are not recommended for use in production applications. To determine whether an API is available in v1.0, use the Version selector

> **Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.



## Properties
|Property|Type|Description|
|:---|:---|:---|
|settingName|String|Setting name specified in the rule.|
|operator|[operator](../resources/intune-deviceconfig-operator.md)|Operator specified in the rule. Possible values are: `none`, `and`, `or`, `isEquals`, `notEquals`, `greaterThan`, `lessThan`, `between`, `notBetween`, `greaterEquals`, `lessEquals`, `dayTimeBetween`, `beginsWith`, `notBeginsWith`, `endsWith`, `notEndsWith`, `contains`, `notContains`, `allOf`, `oneOf`, `noneOf`, `setEquals`, `orderedSetEquals`, `subsetOf`, `excludesAll`.|
|deviceComplianceScriptRulOperator|[deviceComplianceScriptRulOperator](../resources/intune-deviceconfig-devicecompliancescriptruloperator.md)|Operator specified in the rule. Possible values are: `none`, `and`, `or`, `isEquals`, `notEquals`, `greaterThan`, `lessThan`, `between`, `notBetween`, `greaterEquals`, `lessEquals`, `dayTimeBetween`, `beginsWith`, `notBeginsWith`, `endsWith`, `notEndsWith`, `contains`, `notContains`, `allOf`, `oneOf`, `noneOf`, `setEquals`, `orderedSetEquals`, `subsetOf`, `excludesAll`.|
|dataType|[dataType](../resources/intune-deviceconfig-datatype.md)|Data type specified in the rule. Possible values are: `none`, `boolean`, `int64`, `double`, `string`, `dateTime`, `version`, `base64`, `xml`, `booleanArray`, `int64Array`, `doubleArray`, `stringArray`, `dateTimeArray`, `versionArray`.|
|deviceComplianceScriptRuleDataType|[deviceComplianceScriptRuleDataType](../resources/intune-deviceconfig-devicecompliancescriptruledatatype.md)|Data type specified in the rule. Possible values are: `none`, `boolean`, `int64`, `double`, `string`, `dateTime`, `version`, `base64`, `xml`, `booleanArray`, `int64Array`, `doubleArray`, `stringArray`, `dateTimeArray`, `versionArray`.|
|operand|String|Operand specified in the rule.|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceComplianceScriptRule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceComplianceScriptRule",
  "settingName": "String",
  "operator": "String",
  "deviceComplianceScriptRulOperator": "String",
  "dataType": "String",
  "deviceComplianceScriptRuleDataType": "String",
  "operand": "String"
}
```