---
title: "macOSSystemExtensionType enum type"
description: "Flag enum representing the allowed macOS system extension types."
author: "jaiprakashmb"
ms.localizationpriority: medium
ms.subservice: "intune"
doc_type: enumPageType
ms.date: 08/01/2024
---

# macOSSystemExtensionType enum type

Namespace: microsoft.graph

> **Important:** APIs under the /beta version in Microsoft Graph are subject to change which could break your applications. While Intune /beta APIs are supported by Microsoft, you should use these at your own discretion. In general, /beta APIs are not recommended for use in production applications. To determine whether an API is available in v1.0, use the Version selector

> **Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.

Flag enum representing the allowed macOS system extension types.

## Members
|Member|Value|Description|
|:---|:---|:---|
|driverExtensionsAllowed|1|Enables driver extensions.|
|networkExtensionsAllowed|2|Enables network extensions.|
|endpointSecurityExtensionsAllowed|4|Enables endpoint security extensions.|