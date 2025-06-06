---
title: "mobileAppContentFileUploadState enum type"
description: "Contains properties for upload request states."
author: "jaiprakashmb"
ms.localizationpriority: medium
ms.subservice: "intune"
doc_type: enumPageType
ms.date: 08/01/2024
---

# mobileAppContentFileUploadState enum type

Namespace: microsoft.graph

> **Important:** APIs under the /beta version in Microsoft Graph are subject to change which could break your applications. While Intune /beta APIs are supported by Microsoft, you should use these at your own discretion. In general, /beta APIs are not recommended for use in production applications. To determine whether an API is available in v1.0, use the Version selector

> **Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.

Contains properties for upload request states.

## Members
|Member|Value|Description|
|:---|:---|:---|
|success|0||
|transientError|1||
|error|2||
|unknown|3||
|azureStorageUriRequestSuccess|100||
|azureStorageUriRequestPending|101||
|azureStorageUriRequestFailed|102||
|azureStorageUriRequestTimedOut|103||
|azureStorageUriRenewalSuccess|200||
|azureStorageUriRenewalPending|201||
|azureStorageUriRenewalFailed|202||
|azureStorageUriRenewalTimedOut|203||
|commitFileSuccess|300||
|commitFilePending|301||
|commitFileFailed|302||
|commitFileTimedOut|303||