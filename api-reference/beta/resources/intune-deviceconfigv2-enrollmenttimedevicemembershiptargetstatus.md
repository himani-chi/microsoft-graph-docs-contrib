---
title: "enrollmentTimeDeviceMembershipTargetStatus resource type"
description: "Represents the Validation status of the device membership targets. The set/get EnrollmentTimeDeviceMembershipTarget API validates the device membership targets specified by the admin to ensure that they exist, that they are of the proper type, and any other target requirements are met such as that the Intune Device Provisioning First Party App is an owner of the target."
author: "jaiprakashmb"
ms.localizationpriority: medium
ms.subservice: "intune"
doc_type: resourcePageType
ms.date: 08/01/2024
---

# enrollmentTimeDeviceMembershipTargetStatus resource type

Namespace: microsoft.graph
> **Important:** APIs under the /beta version in Microsoft Graph are subject to change which could break your applications. While Intune /beta APIs are supported by Microsoft, you should use these at your own discretion. In general, /beta APIs are not recommended for use in production applications. To determine whether an API is available in v1.0, use the Version selector.

> **Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.


Represents the Validation status of the device membership targets. The set/get EnrollmentTimeDeviceMembershipTarget API validates the device membership targets specified by the admin to ensure that they exist, that they are of the proper type, and any other target requirements are met such as that the Intune Device Provisioning First Party App is an owner of the target.

## Properties
|Property|Type|Description|
|:---|:---|:---|
|targetId|String|The unique identifiers of the targets that devices will become members of when enrolled with the asociated profile.|
|validationSucceeded|Boolean|Indicates if validations succeeded for the device membership target. When 'true', the device membership target validation found no issues. When 'false', the device membership target validation found issues. default - false|
|targetValidationErrorCode|[enrollmentTimeDeviceMembershipTargetValidationErrorCode](../resources/intune-deviceconfigv2-enrollmenttimedevicemembershiptargetvalidationerrorcode.md)|The Validation Error of target that devices will become members of when enrolled with the asociated profile. When there are validation issues are found this property is set with the associated error code of the failure and validationSucceeded property is set to is false. When there are no validation issues found this property will have default value: unknown and validationSucceeded property is set to is true. Possible validation values are unknown,securityGroupNotFound,notSecurityGroup,notStaticSecurityGroup,firstPartyAppNotAnOwner. Default value : unknown. Possible values are: `unknown`, `securityGroupNotFound`, `notSecurityGroup`, `notStaticSecurityGroup`, `firstPartyAppNotAnOwner`, `securityGroupNotInCallerScope`, `unknownFutureValue`.|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.enrollmentTimeDeviceMembershipTargetStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.enrollmentTimeDeviceMembershipTargetStatus",
  "targetId": "String",
  "validationSucceeded": true,
  "targetValidationErrorCode": "String"
}
```
