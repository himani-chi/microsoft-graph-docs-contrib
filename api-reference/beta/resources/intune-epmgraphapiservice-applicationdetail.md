---
title: "applicationDetail resource type"
description: "The details of the application which the user has requested to elevate"
author: "jaiprakashmb"
ms.localizationpriority: medium
ms.subservice: "intune"
doc_type: resourcePageType
ms.date: 08/01/2024
---

# applicationDetail resource type

Namespace: microsoft.graph

> **Important:** APIs under the /beta version in Microsoft Graph are subject to change which could break your applications. While Intune /beta APIs are supported by Microsoft, you should use these at your own discretion. In general, /beta APIs are not recommended for use in production applications. To determine whether an API is available in v1.0, use the Version selector.

> **Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.

The details of the application which the user has requested to elevate

## Properties
|Property|Type|Description|
|:---|:---|:---|
|fileHash|String|The SHA256 hash of the file in the request for elevation, for example, '18ee24150dcb1d96752a4d6dd0f20dfd8ba8c38527e40aa8509b7adecf78f9c6'|
|fileName|String|The name of the file in the request for elevation, for example, git.exe|
|filePath|String|The path of the file in the request for elevation, for example, %programfiles%\git\cmd|
|fileDescription|String|The path of the file in the request for elevation, for example, %programfiles%\git\cmd|
|publisherName|String|The certificate issuer name of the certificate used to sign the application, for example, 'Sectigo Public Code Signing CA R36'|
|publisherCert|String|The list of base64 encoded certificate for each signer, for example, string\[encoded_leaf_cert1, encoded_leaf_cert2....\]|
|productName|String|The product name of the application for which elevation request has been made. For example, 'Git'|
|productInternalName|String|The internal name of the application for which elevation request has been made. For example, 'git'|
|productVersion|String|The product version of the application for which elevation request has been made. For example, '2.40.1.0'|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.applicationDetail"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.applicationDetail",
  "fileHash": "String",
  "fileName": "String",
  "filePath": "String",
  "fileDescription": "String",
  "publisherName": "String",
  "publisherCert": "String",
  "productName": "String",
  "productInternalName": "String",
  "productVersion": "String"
}
```
