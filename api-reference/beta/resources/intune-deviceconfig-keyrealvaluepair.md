---
title: "keyRealValuePair resource type"
description: "A key-value pair with a string key and a real (floating-point) value."
author: "jaiprakashmb"
ms.localizationpriority: medium
ms.subservice: "intune"
doc_type: resourcePageType
ms.date: 08/01/2024
---

# keyRealValuePair resource type

Namespace: microsoft.graph

> **Important:** APIs under the /beta version in Microsoft Graph are subject to change which could break your applications. While Intune /beta APIs are supported by Microsoft, you should use these at your own discretion. In general, /beta APIs are not recommended for use in production applications. To determine whether an API is available in v1.0, use the Version selector

> **Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.

A key-value pair with a string key and a real (floating-point) value.


Inherits from [keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|key|String|The string key of the key-value pair. Inherited from [keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)|
|value|Double|The real (floating-point) value of the key-value pair.|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.keyRealValuePair"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.keyRealValuePair",
  "key": "String",
  "value": "4.2"
}
```