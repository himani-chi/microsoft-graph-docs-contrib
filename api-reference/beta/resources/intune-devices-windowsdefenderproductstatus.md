---
title: "windowsDefenderProductStatus enum type"
description: "Product Status of Windows Defender"
author: "jaiprakashmb"
ms.localizationpriority: medium
ms.subservice: "intune"
doc_type: enumPageType
ms.date: 08/01/2024
---

# windowsDefenderProductStatus enum type

Namespace: microsoft.graph

> **Important:** APIs under the /beta version in Microsoft Graph are subject to change which could break your applications. While Intune /beta APIs are supported by Microsoft, you should use these at your own discretion. In general, /beta APIs are not recommended for use in production applications. To determine whether an API is available in v1.0, use the Version selector

> **Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.

Product Status of Windows Defender

## Members
|Member|Value|Description|
|:---|:---|:---|
|noStatus|0|No status|
|serviceNotRunning|1|Service not running|
|serviceStartedWithoutMalwareProtection|2|Service started without any malware protection engine|
|pendingFullScanDueToThreatAction|4|Pending full scan due to threat action|
|pendingRebootDueToThreatAction|8|Pending reboot due to threat action|
|pendingManualStepsDueToThreatAction|16|Pending manual steps due to threat action |
|avSignaturesOutOfDate|32|AV signatures out of date|
|asSignaturesOutOfDate|64|AS signatures out of date|
|noQuickScanHappenedForSpecifiedPeriod|128|No quick scan has happened for a specified period|
|noFullScanHappenedForSpecifiedPeriod|256|No full scan has happened for a specified period|
|systemInitiatedScanInProgress|512|System initiated scan in progress|
|systemInitiatedCleanInProgress|1024|System initiated clean in progress|
|samplesPendingSubmission|2048|There are samples pending submission|
|productRunningInEvaluationMode|4096|Product running in evaluation mode|
|productRunningInNonGenuineMode|8192|Product running in non-genuine Windows mode|
|productExpired|16384|Product expired|
|offlineScanRequired|32768|Off-line scan required|
|serviceShutdownAsPartOfSystemShutdown|65536|Service is shutting down as part of system shutdown|
|threatRemediationFailedCritically|131072|Threat remediation failed critically|
|threatRemediationFailedNonCritically|262144|Threat remediation failed non-critically|
|noStatusFlagsSet|524288|No status flags set (well initialized state)|
|platformOutOfDate|1048576|Platform is out of date|
|platformUpdateInProgress|2097152|Platform update is in progress|
|platformAboutToBeOutdated|4194304|Platform is about to be outdated|
|signatureOrPlatformEndOfLifeIsPastOrIsImpending|8388608|Signature or platform end of life is past or is impending|
|windowsSModeSignaturesInUseOnNonWin10SInstall|16777216|Windows SMode signatures still in use on non-Win10S install|