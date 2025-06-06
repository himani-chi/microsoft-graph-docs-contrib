---
title: "Update deviceManagement"
description: "Update the properties of a deviceManagement object."
author: "jaiprakashmb"
ms.localizationpriority: medium
ms.subservice: "intune"
doc_type: apiPageType
ms.date: 08/01/2024
---

# Update deviceManagement

Namespace: microsoft.graph

> **Important:** APIs under the /beta version in Microsoft Graph are subject to change which could break your applications. While Intune /beta APIs are supported by Microsoft, you should use these at your own discretion. In general, /beta APIs are not recommended for use in production applications. To determine whether an API is available in v1.0, use the Version selector.

> **Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.

Update the properties of a [deviceManagement](../resources/intune-troubleshooting-devicemanagement.md) object.

[!INCLUDE [national-cloud-support](../../includes/all-clouds.md)]

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

|Permission type|Permissions (from least to most privileged)|
|:---|:---|
|Delegated (work or school account)|DeviceManagementConfiguration.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All|
|Delegated (personal Microsoft account)|Not supported.|
|Application|DeviceManagementConfiguration.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All|

## HTTP Request
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}. Required. Learn more about [authentication and authorization](/graph/auth/auth-concepts).|
|Accept|application/json|

## Request body
In the request body, supply a JSON representation for the [deviceManagement](../resources/intune-troubleshooting-devicemanagement.md) object.

The following table shows the properties that are required when you create the [deviceManagement](../resources/intune-troubleshooting-devicemanagement.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String||
|connectorStatus|[connectorStatusDetails](../resources/intune-troubleshooting-connectorstatusdetails.md) collection|The list of connector status for the tenant.|



## Response
If successful, this method returns a `200 OK` response code and an updated [deviceManagement](../resources/intune-troubleshooting-devicemanagement.md) object in the response body.

## Example

### Request
Here is an example of the request.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement
Content-type: application/json
Content-length: 369

{
  "@odata.type": "#microsoft.graph.deviceManagement",
  "connectorStatus": [
    {
      "@odata.type": "microsoft.graph.connectorStatusDetails",
      "connectorName": "vppTokenExpirationDateTime",
      "connectorInstanceId": "Connector Instance Id value",
      "status": "warning",
      "eventDateTime": "2016-12-31T23:59:23.3984029-08:00"
    }
  ]
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 418

{
  "@odata.type": "#microsoft.graph.deviceManagement",
  "id": "0b283420-3420-0b28-2034-280b2034280b",
  "connectorStatus": [
    {
      "@odata.type": "microsoft.graph.connectorStatusDetails",
      "connectorName": "vppTokenExpirationDateTime",
      "connectorInstanceId": "Connector Instance Id value",
      "status": "warning",
      "eventDateTime": "2016-12-31T23:59:23.3984029-08:00"
    }
  ]
}
```
