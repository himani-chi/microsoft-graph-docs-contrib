---
title: "certificateIssuanceStates enum type"
description: "Certificate Issuance State Options."
author: "jaiprakashmb"
ms.localizationpriority: medium
ms.subservice: "intune"
doc_type: enumPageType
ms.date: 08/01/2024
---

# certificateIssuanceStates enum type

Namespace: microsoft.graph

> **Important:** APIs under the /beta version in Microsoft Graph are subject to change which could break your applications. While Intune /beta APIs are supported by Microsoft, you should use these at your own discretion. In general, /beta APIs are not recommended for use in production applications. To determine whether an API is available in v1.0, use the Version selector

> **Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.

Certificate Issuance State Options.

## Members
|Member|Value|Description|
|:---|:---|:---|
|unknown|0||
|challengeIssued|1||
|challengeIssueFailed|2||
|requestCreationFailed|3||
|requestSubmitFailed|4||
|challengeValidationSucceeded|5||
|challengeValidationFailed|6||
|issueFailed|7||
|issuePending|8||
|issued|9||
|responseProcessingFailed|10||
|responsePending|11||
|enrollmentSucceeded|12||
|enrollmentNotNeeded|13||
|revoked|14||
|removedFromCollection|15||
|renewVerified|16||
|installFailed|17||
|installed|18||
|deleteFailed|19||
|deleted|20||
|renewalRequested|21||
|requested|22||