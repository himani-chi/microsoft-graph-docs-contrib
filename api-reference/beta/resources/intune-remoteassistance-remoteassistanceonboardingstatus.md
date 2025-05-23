---
title: "remoteAssistanceOnboardingStatus enum type"
description: "The current TeamViewer connector status"
author: "jaiprakashmb"
ms.localizationpriority: medium
ms.subservice: "intune"
doc_type: enumPageType
ms.date: 08/01/2024
---

# remoteAssistanceOnboardingStatus enum type

Namespace: microsoft.graph

> **Important:** APIs under the /beta version in Microsoft Graph are subject to change which could break your applications. While Intune /beta APIs are supported by Microsoft, you should use these at your own discretion. In general, /beta APIs are not recommended for use in production applications. To determine whether an API is available in v1.0, use the Version selector

> **Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.

The current TeamViewer connector status

## Members
|Member|Value|Description|
|:---|:---|:---|
|notOnboarded|0|The status reported when there is no active TeamViewer connector configured or active|
|onboarding|1|The status reported when the system has initiated a TeamViewer connection, but the service has not yet completed the confirmation of a connector|
|onboarded|2|The status reported when the system has successfully exchanged account information with TeamViewer and can now initiate remote assistance sessions with clients|