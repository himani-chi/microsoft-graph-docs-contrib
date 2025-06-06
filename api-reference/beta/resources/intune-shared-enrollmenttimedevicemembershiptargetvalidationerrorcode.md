---
title: "enrollmentTimeDeviceMembershipTargetValidationErrorCode enum type"
description: "Represents the Validation error of the device membership target.The API will validate the device membership targets specified by the admin to ensure that they exist, that they are of the proper type, and any other target requirements are met such as that the Intune Device Provisioning First Party App is an owner of the target."
author: "jaiprakashmb"
ms.localizationpriority: medium
ms.subservice: "intune"
doc_type: enumPageType
ms.date: 09/12/2024
---

# enrollmentTimeDeviceMembershipTargetValidationErrorCode enum type

Namespace: microsoft.graph

> **Important:** APIs under the /beta version in Microsoft Graph are subject to change which could break your applications. While Intune /beta APIs are supported by Microsoft, you should use these at your own discretion. In general, /beta APIs are not recommended for use in production applications. To determine whether an API is available in v1.0, use the Version selector.

> **Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.

Represents the Validation error of the device membership target.The API will validate the device membership targets specified by the admin to ensure that they exist, that they are of the proper type, and any other target requirements are met such as that the Intune Device Provisioning First Party App is an owner of the target.

## Members
|Member|Value|Description|
|:---|:---|:---|
|unknown|0|Default. Indicates the status of device membership target is not specified. Do not use.|
|securityGroupNotFound|1|Indicates device membership target cannot be found.|
|notSecurityGroup|2|Indicates device membership target is not a security group.|
|notStaticSecurityGroup|3|Indicates device membership target which is security group but not a static one.|
|firstPartyAppNotAnOwner|4|Indicates required first party app not the owner of that device membership target.|
|securityGroupNotInCallerScope|5|Indicates that device membership target of type security group is not in the RBAC scope of the caller.|
|unknownFutureValue|6|Evolvable enumeration sentinel value. Do not use.|
