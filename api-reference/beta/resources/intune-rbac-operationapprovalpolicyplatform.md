---
title: "operationApprovalPolicyPlatform enum type"
description: "The set of available platforms for the OperationApprovalPolicy. Allows configuration of a policy to specific platform(s) for approval. If no specific platform is required or applicable, the platform is `notApplicable`."
author: "jaiprakashmb"
ms.localizationpriority: medium
ms.subservice: "intune"
doc_type: enumPageType
ms.date: 08/01/2024
---

# operationApprovalPolicyPlatform enum type

Namespace: microsoft.graph

> **Important:** APIs under the /beta version in Microsoft Graph are subject to change which could break your applications. While Intune /beta APIs are supported by Microsoft, you should use these at your own discretion. In general, /beta APIs are not recommended for use in production applications. To determine whether an API is available in v1.0, use the Version selector

> **Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.

The set of available platforms for the OperationApprovalPolicy. Allows configuration of a policy to specific platform(s) for approval. If no specific platform is required or applicable, the platform is `notApplicable`.

## Members
|Member|Value|Description|
|:---|:---|:---|
|notApplicable|0|Default. Indicates that a policy platform is not required for a chosen policy type.|
|androidDeviceAdministrator|1|Indicates that the configured policy platform is for Android Device Administrator.|
|androidEnterprise|2|Indicates that the configured policy platform is for Android Enterprise.|
|iOSiPadOS|4|Indicates that the configured policy platform is for iOS/iPadOS.|
|macOS|8|Indicates that the configured policy platform is for macOS.|
|windows10AndLater|16|Indicates that the configured policy platform is for Windows 10 and later.|
|windows81AndLater|32|Indicates that the configured policy platform is for Windows 8.1 and later.|
|windows10X|64|Indicates that the configured policy platform is for Windows 10X.|
|unknownFutureValue|128|Evolvable enumeration sentinel value. Do not use.|