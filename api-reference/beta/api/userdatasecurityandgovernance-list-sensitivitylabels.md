---
title: "List sensitivityLabels"
description: "List the sensitivity labels available to a specific user"
author: "ArunGedela"
ms.date: 04/21/2025
ms.localizationpriority: medium
ms.subservice: "security"
doc_type: apiPageType
---

# List sensitivityLabels

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

List the sensitivity labels available to a specific user.

## Permissions

Choose the permission or permissions marked as least privileged for this API. Use a higher privileged permission or permissions [only if your app requires it](/graph/permissions-overview#best-practices-for-using-microsoft-graph-permissions). For details about delegated and application permissions, see [Permission types](/graph/permissions-overview#permission-types). To learn more about these permissions, see the [permissions reference](/graph/permissions-reference).

<!-- { "blockType": "permissions", "name": "purviewecosystem-sensitivitylabels-getsensitivitylabels-permissions" } -->
[!INCLUDE [permissions-table](../includes/permissions/userdatasecurityandgovernance-list-sensitivitylabels-permissions.md)]

When using application permissions (`SensitivityLabels.Read.All`), the API returns all labels for the tenant by default. Use the `scopeToUser` query parameter to retrieve labels for a specific user in the application context.


## HTTP request

Get labels for a specific user:

```http
GET /users/{usersId}/dataSecurityAndGovernance/sensitivityLabels
```

## Request headers

| Name                | Description                                                                                                                                 |
| :------------------ | :------------------------------------------------------------------------------------------------------------------------------------------ |
| Authorization       | Bearer {token}. Required. Learn more about [authentication and authorization](/graph/auth/auth-concepts).                                |
| Client-Request-Id   | Optional. A client-generated GUID to trace the request. Recommended for troubleshooting.                                                  |

## Query parameters

| Parameter      | Type             | Description                                                                                                                                                                                                                                                                                           |
| :------------- | :--------------- | :---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| isScopedToUser | Boolean          | Optional. Used only with application permissions (`/security/...` path). If value set to 'true' to scope labels to the current user. If omitted with application permissions, returns all tenant labels. |
| locale         | String           | Optional. Specifies the locale for localizable fields.                                                                                                                                        |
| applicableTo   | String           | Optional. A comma-separated string of content formats (for example, `File,Email`). Filters the returned labels to only those applicable to *at least one* of the specified formats. Possible values are `Email`,`File`,`SchematizedData`,`Site`,`Teamwork`,`UnifiedGroup`. |
| id             | String           | Optional. A comma-separated string of sensitivity label GUIDs. Filters the returned labels to only those matching the specified IDs. |

## Request body

Don't supply a request body for this method.

## Response

If successful, this method returns a `200 OK` response code and a collection of [sensitivityLabel](../resources/security-sensitivitylabel.md) objects in the response body.

## Examples

Get tenant labels filtered by content format and ID with an application permission.

#### Request

The following example shows a request to get labels for the tenant, filtered for the `File` content format and specific IDs.

<!-- {
  "blockType": "request",
  "name": "get_sensitivitylabels_user_filtered_app"
} -->
```http
GET https://graph.microsoft.com/beta/security/dataSecurityAndGovernance/sensitivityLabels?$filter=applicableTo eq 'File' and id in ('4e4234dd-377b-42a3-935b-0e42f138fa23','b7a21bba-8197-491f-a5d6-0d0f955397ca')
Authorization: Bearer {token}
Client-Request-Id: a0b9c8d7-e6f5-a4b3-c2d1-e0f9a8b7c6d5
```

#### Response

The following example shows the response containing only the labels matching the filters.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.security.sensitivityLabel)"
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#security/dataSecurityAndGovernance/sensitivityLabel",
  "value": [
    {
      "id": "4e4234dd-377b-42a3-935b-0e42f138fa23",
      "name": "General",
      "description": "General data, not for public use.",
      "color": "#000000",
      "priority": 10,
      "toolTip": "Apply this label to general non-public data.",
      "isEnabled": true,
      "isEndpointProtectionEnabled": true,
      "autoTooltip": "",
      "isSmimeSignEnabled": true,
      "isSmimeEncryptEnabled": true,
      "actionSource": "manual",
      "applicableTo": "email,teamwork,file",
      "sublabels": []
    }
  ]
}
```
