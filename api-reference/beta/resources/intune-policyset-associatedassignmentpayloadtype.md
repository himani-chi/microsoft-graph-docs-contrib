---
title: "associatedAssignmentPayloadType enum type"
description: "This enum represents associated assignment payload type"
author: "jaiprakashmb"
ms.localizationpriority: medium
ms.subservice: "intune"
doc_type: enumPageType
ms.date: 08/01/2024
---

# associatedAssignmentPayloadType enum type

Namespace: microsoft.graph

> **Important:** APIs under the /beta version in Microsoft Graph are subject to change which could break your applications. While Intune /beta APIs are supported by Microsoft, you should use these at your own discretion. In general, /beta APIs are not recommended for use in production applications. To determine whether an API is available in v1.0, use the Version selector

> **Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.

This enum represents associated assignment payload type

## Members
|Member|Value|Description|
|:---|:---|:---|
|unknown|0|Invalid payload type|
|deviceConfigurationAndCompliance|1|Indicates that this filter is associated with a configuration or compliance policy payload type|
|application|2|Indicates that this assignment filter is associated with an application payload type|
|androidEnterpriseApp|8|Indicates that this filter is associated with a Android Enterprise application payload type|
|enrollmentConfiguration|9|Indicates that this filter is associated with an enrollment restriction or enrollment status page policy payload type|
|groupPolicyConfiguration|12|Indicates that this filter is associated with an Administrative Template policy payload type|
|zeroTouchDeploymentDeviceConfigProfile|15|Indicates that this assignment filter is associated with Zero touch deployment Device Configuration Profile payload type|
|androidEnterpriseConfiguration|16|Indicates that this filter is associated with an Android Enterprise Configuration policy payload type|
|deviceFirmwareConfigurationInterfacePolicy|20|Indicates that this assignment filter is associated with Device Firmware Configuration Interface(DCFI) payload type|
|resourceAccessPolicy|23|Indicates that this filter is associated with a resource access policy (Wifi, VPN, Certificate) payload type|
|win32app|24|Indicates that this filter is associated with a Win32 app payload type|
|deviceManagmentConfigurationAndCompliancePolicy|29|Indicates that this filter is associated with a configuration or compliance policy on Device Configuration v2 Infrastructure payload type|