---
title: "webCategoryFilteringRule resource type"
description: "Defines a network filtering rule for web categories, enabling administrators to manage access to specific categories of websites."
author: "Moti-ba"
ms.localizationpriority: medium
ms.subservice: "entra-global-secure-access"
doc_type: resourcePageType
ms.date: 09/23/2024
---

# webCategoryFilteringRule resource type

Namespace: microsoft.graph.networkaccess

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Defines a network filtering rule for web categories, enabling administrators to manage access to specific categories of websites.

Inherits from [filteringRule](../resources/networkaccess-filteringrule.md).

## Methods
None.

For the list of API operations for managing this resource type, see [filteringRule](../resources/networkaccess-filteringrule.md).

## Properties
|Property|Type|Description|
|:---|:---|:---|
|destinations|[microsoft.graph.networkaccess.ruleDestination](../resources/networkaccess-ruledestination.md) collection|The list of potential destinations and destination types that the user may access, including fully qualified domain names (FQDNs) and web categories, within the context of a network filtering policy. Inherited from [microsoft.graph.networkaccess.filteringRule](../resources/networkaccess-filteringrule.md).|
|id|String|The unique identifier for the **webCategoryFilteringRule**. Inherited from [microsoft.graph.networkaccess.filteringRule](../resources/networkaccess-filteringrule.md).|
|name|String|Display name. Inherited from [microsoft.graph.networkaccess.filteringRule](../resources/networkaccess-filteringrule.md).|
|ruleType|microsoft.graph.networkaccess.networkDestinationType|The network destination type used by a filtering rule. Supports a subset of the values for **networkDestinationType**. The possible values are: `fqdn`, `webCategory`, `unknownFutureValue`. Inherited from [microsoft.graph.networkaccess.filteringRule](../resources/networkaccess-filteringrule.md). |

## Relationships
None.

## JSON representation
The following JSON representation shows the resource type.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.networkaccess.webCategoryFilteringRule",
  "baseType": "microsoft.graph.networkaccess.filteringRule",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.networkaccess.webCategoryFilteringRule",
  "destinations": [{"@odata.type": "microsoft.graph.networkaccess.ruleDestination"}],
  "id": "String (identifier)",
  "name": "String",
  "ruleType": "String"
}
```

