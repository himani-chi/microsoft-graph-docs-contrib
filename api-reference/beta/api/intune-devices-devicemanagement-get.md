---
title: "Get deviceManagement"
description: "Read properties and relationships of the deviceManagement object."
author: "jaiprakashmb"
ms.localizationpriority: medium
ms.subservice: "intune"
doc_type: apiPageType
ms.date: 08/01/2024
---

# Get deviceManagement

Namespace: microsoft.graph

> **Important:** APIs under the /beta version in Microsoft Graph are subject to change which could break your applications. While Intune /beta APIs are supported by Microsoft, you should use these at your own discretion. In general, /beta APIs are not recommended for use in production applications. To determine whether an API is available in v1.0, use the Version selector.

> **Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.

Read properties and relationships of the [deviceManagement](../resources/intune-devices-devicemanagement.md) object.

[!INCLUDE [national-cloud-support](../../includes/all-clouds.md)]

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

|Permission type|Permissions (from least to most privileged)|
|:---|:---|
|Delegated (work or school account)|DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All, DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All|
|Delegated (personal Microsoft account)|Not supported.|
|Application|DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All, DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All|

## HTTP Request
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement
```

## Optional query parameters
This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}. Required. Learn more about [authentication and authorization](/graph/auth/auth-concepts).|
|Accept|application/json|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and [deviceManagement](../resources/intune-devices-devicemanagement.md) object in the response body.

## Example

### Request
Here is an example of the request.
``` http
GET https://graph.microsoft.com/beta/deviceManagement
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 4109

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagement",
    "id": "0b283420-3420-0b28-2034-280b2034280b",
    "subscriptionState": "active",
    "subscriptions": "intune",
    "managedDeviceCleanupSettings": {
      "@odata.type": "microsoft.graph.managedDeviceCleanupSettings",
      "deviceInactivityBeforeRetirementInDays": "Device Inactivity Before Retirement In Days value"
    },
    "adminConsent": {
      "@odata.type": "microsoft.graph.adminConsent",
      "shareAPNSData": "granted",
      "shareUserExperienceAnalyticsData": "granted"
    },
    "deviceProtectionOverview": {
      "@odata.type": "microsoft.graph.deviceProtectionOverview",
      "totalReportedDeviceCount": 8,
      "inactiveThreatAgentDeviceCount": 14,
      "unknownStateThreatAgentDeviceCount": 2,
      "pendingSignatureUpdateDeviceCount": 1,
      "cleanDeviceCount": 0,
      "pendingFullScanDeviceCount": 10,
      "pendingRestartDeviceCount": 9,
      "pendingManualStepsDeviceCount": 13,
      "pendingOfflineScanDeviceCount": 13,
      "criticalFailuresDeviceCount": 11,
      "pendingQuickScanDeviceCount": 11
    },
    "windowsMalwareOverview": {
      "@odata.type": "microsoft.graph.windowsMalwareOverview",
      "malwareDetectedDeviceCount": 10,
      "totalMalwareCount": 1,
      "totalDistinctMalwareCount": 9,
      "malwareStateSummary": [
        {
          "@odata.type": "microsoft.graph.windowsMalwareStateCount",
          "state": "actionFailed",
          "deviceCount": 11,
          "malwareDetectionCount": 5,
          "distinctMalwareCount": 4,
          "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00"
        }
      ],
      "malwareSeveritySummary": [
        {
          "@odata.type": "microsoft.graph.windowsMalwareSeverityCount",
          "severity": "low",
          "malwareDetectionCount": 5,
          "distinctMalwareCount": 4,
          "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00"
        }
      ],
      "malwareExecutionStateSummary": [
        {
          "@odata.type": "microsoft.graph.windowsMalwareExecutionStateCount",
          "executionState": "blocked",
          "deviceCount": 11,
          "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00"
        }
      ],
      "malwareCategorySummary": [
        {
          "@odata.type": "microsoft.graph.windowsMalwareCategoryCount",
          "category": "adware",
          "deviceCount": 11,
          "activeMalwareDetectionCount": 11,
          "distinctActiveMalwareCount": 10,
          "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00"
        }
      ],
      "malwareNameSummary": [
        {
          "@odata.type": "microsoft.graph.windowsMalwareNameCount",
          "malwareIdentifier": "Malware Identifier value",
          "name": "Name value",
          "deviceCount": 11,
          "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00"
        }
      ],
      "osVersionsSummary": [
        {
          "@odata.type": "microsoft.graph.osVersionCount",
          "osVersion": "Os Version value",
          "deviceCount": 11,
          "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00"
        }
      ]
    },
    "accountMoveCompletionDateTime": "2017-01-01T00:01:17.9006709-08:00",
    "userExperienceAnalyticsSettings": {
      "@odata.type": "microsoft.graph.userExperienceAnalyticsSettings",
      "configurationManagerDataConnectorConfigured": true
    },
    "dataProcessorServiceForWindowsFeaturesOnboarding": {
      "@odata.type": "microsoft.graph.dataProcessorServiceForWindowsFeaturesOnboarding",
      "hasValidWindowsLicense": true,
      "areDataProcessorServiceForWindowsFeaturesEnabled": true
    },
    "userExperienceAnalyticsAnomalySeverityOverview": {
      "@odata.type": "microsoft.graph.userExperienceAnalyticsAnomalySeverityOverview",
      "lowSeverityAnomalyCount": 7,
      "mediumSeverityAnomalyCount": 10,
      "highSeverityAnomalyCount": 8,
      "informationalSeverityAnomalyCount": 1
    }
  }
}
```
