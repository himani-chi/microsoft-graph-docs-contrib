---
title: "firewallCertificateRevocationListCheckMethodType enum type"
description: "Possible values for firewallCertificateRevocationListCheckMethod"
author: "jaiprakashmb"
ms.localizationpriority: medium
ms.subservice: "intune"
doc_type: enumPageType
ms.date: 08/01/2024
---

# firewallCertificateRevocationListCheckMethodType enum type

Namespace: microsoft.graph

> **Important:** APIs under the /beta version in Microsoft Graph are subject to change which could break your applications. While Intune /beta APIs are supported by Microsoft, you should use these at your own discretion. In general, /beta APIs are not recommended for use in production applications. To determine whether an API is available in v1.0, use the Version selector

> **Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.

Possible values for firewallCertificateRevocationListCheckMethod

## Members
|Member|Value|Description|
|:---|:---|:---|
|deviceDefault|0|No value configured by Intune, do not override the user-configured device default value|
|none|1|Do not check certificate revocation list|
|attempt|2|Attempt CRL check and allow a certificate only if the certificate is confirmed by the check|
|require|3|Require a successful CRL check before allowing a certificate|