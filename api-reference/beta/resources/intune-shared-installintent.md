---
title: "installIntent enum type"
description: "Possible values for the install intent chosen by the admin."
author: "jaiprakashmb"
ms.localizationpriority: medium
ms.subservice: "intune"
doc_type: enumPageType
ms.date: 08/01/2024
---

# installIntent enum type

Namespace: microsoft.graph
> **Important:** APIs under the /beta version in Microsoft Graph are subject to change which could break your applications. While Intune /beta APIs are supported by Microsoft, you should use these at your own discretion. In general, /beta APIs are not recommended for use in production applications. To determine whether an API is available in v1.0, use the Version selector.

> **Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.


Possible values for the install intent chosen by the admin.

## Members
|Member|Value|Description|
|:---|:---|:---|
|available|0|Available install intent.|
|required|1|Required install intent.|
|uninstall|2|Uninstall install intent.|
|availableWithoutEnrollment|3|Available without enrollment install intent.|
