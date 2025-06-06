---
title: "Get awsIdentityAccessManagementKeyUsageFinding"
description: "Read the properties and relationships of an awsIdentityAccessManagementKeyUsageFinding object."
author: "ashyasingh"
ms.reviewer: ciem_pm
ms.localizationpriority: medium
ms.subservice: entra-permissions-management
doc_type: apiPageType
ms.date: 04/18/2024
---

# Get awsIdentityAccessManagementKeyUsageFinding
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [permissions-management-retirement-note](../../includes/permissions-management-retirement-note.md)]

Read the properties and relationships of an [awsIdentityAccessManagementKeyUsageFinding](../resources/awsidentityaccessmanagementkeyusagefinding.md) object.

## Permissions
Choose the permission or permissions marked as least privileged for this API. Use a higher privileged permission or permissions [only if your app requires it](/graph/permissions-overview#best-practices-for-using-microsoft-graph-permissions). For details about delegated and application permissions, see [Permission types](/graph/permissions-overview#permission-types). To learn more about these permissions, see the [permissions reference](/graph/permissions-reference).

<!-- { "blockType": "permissions", "name": "awsidentityaccessmanagementkeyusagefinding_get" } -->
[!INCLUDE [permissions-table](../includes/permissions/awsidentityaccessmanagementkeyusagefinding-get-permissions.md)]

## HTTP request

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/permissionsAnalytics/aws/findings/{id}/microsoft.graph.awsIdentityAcessManagementKeyUsageFinding
```

## Optional query parameters
This method does not support OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required. Learn more about [authentication and authorization](/graph/auth/auth-concepts).|

## Request body
Don't supply a request body for this method.

## Response

If successful, this method returns a `200 OK` response code and an [awsIdentityAccessManagementKeyUsageFinding](../resources/awsidentityaccessmanagementkeyusagefinding.md) object in the response body.

## Examples

### Request
The following example shows a request.
<!-- {
  "blockType": "request",
  "name": "get_awsidentityaccessmanagementkeyusagefinding"
}
-->
``` http
GET https://graph.microsoft.com/beta/identityGovernance/permissionsAnalytics/aws/findings/MSxBd3NJZGVudGl0eUFjY2Vzc01hbmFnZW1lbnRLZXlVc2FnZUZpbmRpbmcsMjEyNjk/microsoft.graph.awsIdentityAcessManagementKeyUsageFinding
```


### Response
The following example shows the response.
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.awsIdentityAccessManagementKeyUsageFinding"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/permissionsAnalytics/aws/findings/microsoft.graph.awsIdentityAccessManagementKeyUsageFinding/$entity",
    "id": "MSxBd3NJZGVudGl0eUFjY2Vzc01hbmFnZW1lbnRLZXlVc2FnZUZpbmRpbmcsMjEyNjk",
    "createdDateTime": "2023-10-25T23:48:12.164332Z",
    "status": "inactive",
    "permissionsCreepIndex": {
        "score": 4
    },
    "actionSummary": {
        "assigned": 4161,
        "exercised": 0,
        "available": 58
    },
    "accessKey": {
        "id": "QUtJQTU1VUhNS0IzM1hTWFRSNjI",
        "externalId": "AKIA55UHMKB33XSXTR62",
        "displayName": "AKIA55UHMKB33XSXTR62",
        "source": {
            "@odata.type": "#microsoft.graph.awsSource",
            "identityProviderType": "aws",
            "accountId": "956987887735"
        },
        "authorizationSystem": {
            "@odata.type": "#microsoft.graph.awsAuthorizationSystem",
            "authorizationSystemId": "956987887735",
            "authorizationSystemName": "ck-development",
            "authorizationSystemType": "aws",
            "id": "MSxhd3MsOTU2OTg3ODg3NzM1"
        },
        "owner": {
            "id": "YXJuOmF3czppYW06Ojk1Njk4Nzg4NzczNTp1c2VyL2FuZHl3YW5n",
            "externalId": "arn:aws:iam::956987887735:user/andywang",
            "displayName": "andywang",
            "source": {
                "@odata.type": "#microsoft.graph.awsSource",
                "identityProviderType": "aws",
                "accountId": "956987887735"
            }
        }
    }
}
```


