---
title: "policySetStatus enum type"
description: "The enum to specify the status of PolicySet."
author: "jaiprakashmb"
ms.localizationpriority: medium
ms.subservice: "intune"
doc_type: enumPageType
ms.date: 08/01/2024
---

# policySetStatus enum type

Namespace: microsoft.graph

> **Important:** APIs under the /beta version in Microsoft Graph are subject to change which could break your applications. While Intune /beta APIs are supported by Microsoft, you should use these at your own discretion. In general, /beta APIs are not recommended for use in production applications. To determine whether an API is available in v1.0, use the Version selector

> **Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.

The enum to specify the status of PolicySet.

## Members
|Member|Value|Description|
|:---|:---|:---|
|unknown|0|Default Value.|
|validating|1|All PolicySet items are now validating for corresponding settings of workloads.|
|partialSuccess|2|Post process complete for all PolicySet items but there are failures.|
|success|3|All PolicySet items are deployed. Doesn’t mean that all deployment succeeded. |
|error|4|PolicySet processing completely failed.|
|notAssigned|5|PolicySet/PolicySetItem is not assigned to any group.|