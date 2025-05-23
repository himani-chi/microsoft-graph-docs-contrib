---
title: "List browserSites"
description: "Get a list of the browserSite objects and their properties."
author: "edward-day-vii"
ms.localizationpriority: medium
ms.subservice: "edge-browser-management"
doc_type: apiPageType
ms.date: 04/04/2024
---

# List browserSites
Namespace: microsoft.graph

Get a list of the [browserSite](../resources/browsersite.md) objects and their properties.

[!INCLUDE [national-cloud-support](../../includes/global-only.md)]

## Permissions
Choose the permission or permissions marked as least privileged for this API. Use a higher privileged permission or permissions [only if your app requires it](/graph/permissions-overview#best-practices-for-using-microsoft-graph-permissions). For details about delegated and application permissions, see [Permission types](/graph/permissions-overview#permission-types). To learn more about these permissions, see the [permissions reference](/graph/permissions-reference).

<!-- { "blockType": "permissions", "name": "browsersitelist_list_sites" } -->
[!INCLUDE [permissions-table](../includes/permissions/browsersitelist-list-sites-permissions.md)]

## HTTP request

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /admin/edge/internetExplorerMode/siteLists/{browserSiteListId}/sites
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required. Learn more about [authentication and authorization](/graph/auth/auth-concepts).|

## Request body
Don't supply a request body for this method.

## Response

If successful, this method returns a `200 OK` response code and a collection of [browserSite](../resources/browsersite.md) objects in the response body.

## Examples

### Request
The following example shows a request.
# [HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_browsersite",
  "sampleKeys": ["e370d818-f650-5ab1-499e-5915e83f4573"]
}
-->
``` http
GET https://graph.microsoft.com/v1.0/admin/edge/internetExplorerMode/siteLists/e370d818-f650-5ab1-499e-5915e83f4573/sites
```

# [C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-browsersite-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [CLI](#tab/cli)
[!INCLUDE [sample-code](../includes/snippets/cli/list-browsersite-cli-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/list-browsersite-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-browsersite-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-browsersite-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [PHP](#tab/php)
[!INCLUDE [sample-code](../includes/snippets/php/list-browsersite-php-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/list-browsersite-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [Python](#tab/python)
[!INCLUDE [sample-code](../includes/snippets/python/list-browsersite-python-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### Response
The following example shows the response.
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.browserSite",
  "isCollection": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "value": [
        {
            "status": "pendingEdit",
            "id": "a22cbc85-d5d2-4e61-8414-42e6704c36f7",
            "webUrl": "www.microsoft.com",
            "targetEnvironment": "microsoftEdge",
            "mergeType": "default",
            "compatibilityMode": "default",
            "allowRedirect": false,
            "comment": "Updating to Edge.",
            "lastModifiedDateTime": "2022-06-29T15:44:27.2154899Z",
            "createdDateTime": "2022-06-29T14:51:23.8662595Z",
            "deletedDateTime": null,
            "lastModifiedBy": {
                "user": {
                    "id": "f6ff107e-bc40-4918-a432-8d7b60030a7c",
                    "displayName": "Joe Smith"
                },
                "application": null
            },
            "history": [
                {
                    "publishedDateTime": "2022-06-29T14:51:23.8662592Z",
                    "allowRedirect": true,
                    "comment": "A site that opens in InternetExplorer11",
                    "compatibilityMode": "default",
                    "targetEnvironment": "internetExplorer11",
                    "mergeType": "default",
                    "lastModifiedBy": {
                        "user": {
                            "id": "f6ff107e-bc40-4918-a432-8d7b60030a7c",
                            "displayName": "Joe Smith"
                        },
                        "application": null
                    }
                }
            ]
        }
    ]
}
```

