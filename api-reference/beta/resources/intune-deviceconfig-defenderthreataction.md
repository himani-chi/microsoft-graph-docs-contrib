---
title: "defenderThreatAction enum type"
description: "Defender’s default action to take on detected Malware threats."
author: "jaiprakashmb"
ms.localizationpriority: medium
ms.subservice: "intune"
doc_type: enumPageType
ms.date: 08/01/2024
---

# defenderThreatAction enum type

Namespace: microsoft.graph

> **Important:** APIs under the /beta version in Microsoft Graph are subject to change which could break your applications. While Intune /beta APIs are supported by Microsoft, you should use these at your own discretion. In general, /beta APIs are not recommended for use in production applications. To determine whether an API is available in v1.0, use the Version selector

> **Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.

Defender’s default action to take on detected Malware threats.

## Members
|Member|Value|Description|
|:---|:---|:---|
|deviceDefault|0|Apply action based on the update definition.|
|clean|1|Clean the detected threat.|
|quarantine|2|Quarantine the detected threat.|
|remove|3|Remove the detected threat.|
|allow|4|Allow the detected threat.|
|userDefined|5|Allow the user to determine the action to take with the detected threat.|
|block|6|Block the detected threat.|