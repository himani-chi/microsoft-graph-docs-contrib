---
title: "iosKioskModeAppType enum type"
description: "App source options for iOS kiosk mode."
author: "jaiprakashmb"
ms.localizationpriority: medium
ms.subservice: "intune"
doc_type: enumPageType
ms.date: 08/01/2024
---

# iosKioskModeAppType enum type

Namespace: microsoft.graph

> **Important:** APIs under the /beta version in Microsoft Graph are subject to change which could break your applications. While Intune /beta APIs are supported by Microsoft, you should use these at your own discretion. In general, /beta APIs are not recommended for use in production applications. To determine whether an API is available in v1.0, use the Version selector

> **Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.

App source options for iOS kiosk mode.

## Members
|Member|Value|Description|
|:---|:---|:---|
|notConfigured|0|Device default value, no intent.|
|appStoreApp|1|The app to be run comes from the app store.|
|managedApp|2|The app to be run is built into the device.|
|builtInApp|3|The app to be run is a managed app.|