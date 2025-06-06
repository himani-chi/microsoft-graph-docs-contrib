---
title: "Get educationAssignmentResource"
description: "Get the properties of a specific resource on an assignment.  "
author: "Sureshpadimi88"
ms.localizationpriority: medium
ms.subservice: "education"
doc_type: apiPageType
ms.date: 04/05/2024
---

# Get educationAssignmentResource

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Get the properties of an [education assignment resource](../resources/educationassignmentresource.md) associated with an [assignment](../resources/educationassignment.md). Only teachers, students, and applications with application permissions can perform this operation.

[!INCLUDE [national-cloud-support](../../includes/global-only.md)]

## Permissions
Choose the permission or permissions marked as least privileged for this API. Use a higher privileged permission or permissions [only if your app requires it](/graph/permissions-overview#best-practices-for-using-microsoft-graph-permissions). For details about delegated and application permissions, see [Permission types](/graph/permissions-overview#permission-types). To learn more about these permissions, see the [permissions reference](/graph/permissions-reference).

<!-- { "blockType": "permissions", "name": "educationassignmentresource_get" } -->
[!INCLUDE [permissions-table](../includes/permissions/educationassignmentresource-get-permissions.md)]

## HTTP request
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{class-id}/assignments/{assignment-id}/resources/{resource-id}
```

## Optional query parameters

This method supports the `$select` OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).


## Request headers
| Header       | Value |
|:---------------|:--------|
|Authorization|Bearer {token}. Required. Learn more about [authentication and authorization](/graph/auth/auth-concepts).|

## Request body
Don't supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and an [educationAssignmentResource](../resources/educationassignmentresource.md) object in the response body.

## Examples
### Example 1: Get an educationWordResource
#### Request
The following example shows a request.


# [HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_educationassignmentresource_e1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/education/classes/72a7baec-c3e9-4213-a850-f62de0adad5f/assignments/1618dfb0-3ff2-4edf-8d5c-b8f81df00e80/resources/fb92ec62-3996-4c3a-ad41-720dd930c834
```

# [C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationassignmentresource-e1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [CLI](#tab/cli)
[!INCLUDE [sample-code](../includes/snippets/cli/get-educationassignmentresource-e1-cli-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-educationassignmentresource-e1-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-educationassignmentresource-e1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationassignmentresource-e1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [PHP](#tab/php)
[!INCLUDE [sample-code](../includes/snippets/php/get-educationassignmentresource-e1-php-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/get-educationassignmentresource-e1-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [Python](#tab/python)
[!INCLUDE [sample-code](../includes/snippets/python/get-educationassignmentresource-e1-python-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### Response
The following example shows the response.

>**Note:** The response object shown here might be shortened for readability.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationWordResource"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#education/classes('72a7baec-c3e9-4213-a850-f62de0adad5f')/assignments('1618dfb0-3ff2-4edf-8d5c-b8f81df00e80')/resources/$entity",
    "distributeForStudentWork": false,
    "id": "fb92ec62-3996-4c3a-ad41-720dd930c834",
    "resource": {
        "@odata.type": "#microsoft.graph.educationWordResource",
        "displayName": "IR Azure function - Next steps.docx",
        "createdDateTime": "2021-09-13T15:51:05.5541912Z",
        "lastModifiedDateTime": "2021-09-13T15:51:05.5541912Z",
        "fileUrl": "https://graph.microsoft.com/beta/drives/b!OPmUsPgnBUiMIXMxWcj3neC1xck6I5NIsnFxfrLdmXoOOmEQNO79QpIMPdOmY3nf/items/01QTY63RLYFJ4KNRTN4FCZVQWKZ6DMKBNP",
        "createdBy": {
            "application": null,
            "device": null,
            "user": {
                "id": "f3a5344e-dbde-48b0-be24-b5b62a243836",
                "displayName": null
            }
        },
        "lastModifiedBy": {
            "application": null,
            "device": null,
            "user": {
                "id": "f3a5344e-dbde-48b0-be24-b5b62a243836",
                "displayName": null
            }
        }
    }
}
    
```

### Example 2: Get an educationLinkResource
#### Request
The following example shows a request.

# [HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["72a7baec-c3e9-4213-a850-f62de0adad5f","1618dfb0-3ff2-4edf-8d5c-b8f81df00e80","a2f95693-aea2-4d5e-a936-11ef390f8f20"], 
  "name": "get_educationlinkresource_from_educationassignment_e2"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/education/classes/72a7baec-c3e9-4213-a850-f62de0adad5f/assignments/1618dfb0-3ff2-4edf-8d5c-b8f81df00e80/resources/a2f95693-aea2-4d5e-a936-11ef390f8f20
```

# [C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationlinkresource-from-educationassignment-e2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [CLI](#tab/cli)
[!INCLUDE [sample-code](../includes/snippets/cli/get-educationlinkresource-from-educationassignment-e2-cli-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-educationlinkresource-from-educationassignment-e2-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-educationlinkresource-from-educationassignment-e2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationlinkresource-from-educationassignment-e2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [PHP](#tab/php)
[!INCLUDE [sample-code](../includes/snippets/php/get-educationlinkresource-from-educationassignment-e2-php-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/get-educationlinkresource-from-educationassignment-e2-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [Python](#tab/python)
[!INCLUDE [sample-code](../includes/snippets/python/get-educationlinkresource-from-educationassignment-e2-python-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### Response
The following example shows the response.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationLinkResource"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#education/classes('72a7baec-c3e9-4213-a850-f62de0adad5f')/assignments('1618dfb0-3ff2-4edf-8d5c-b8f81df00e80')/resources/$entity",
    "distributeForStudentWork": false,
    "id": "a2f95693-aea2-4d5e-a936-11ef390f8f20",
    "resource": {
        "@odata.type": "#microsoft.graph.educationLinkResource",
        "displayName": "Where the Wonders of Learning Never Cease | Wonderopolis",
        "createdDateTime": "2021-09-13T15:50:39.0017937Z",
        "lastModifiedDateTime": "2021-09-13T15:50:39.0017937Z",
        "link": "https://wonderopolis.org/",
        "createdBy": {
            "application": null,
            "device": null,
            "user": {
                "id": "f3a5344e-dbde-48b0-be24-b5b62a243836",
                "displayName": null
            }
        },
        "lastModifiedBy": {
            "application": null,
            "device": null,
            "user": {
                "id": "f3a5344e-dbde-48b0-be24-b5b62a243836",
                "displayName": null
            }
        }
    }
}
```

### Example 3: Get an educationExcelResource
#### Request
The following example shows a request.

# [HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["72a7baec-c3e9-4213-a850-f62de0adad5f","1618dfb0-3ff2-4edf-8d5c-b8f81df00e80","517b36a6-9ca2-4e7b-9748-3af25f5cd4fd"], 
  "name": "get_educationexcelresource_from_educationassignment_e3"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/education/classes/72a7baec-c3e9-4213-a850-f62de0adad5f/assignments/1618dfb0-3ff2-4edf-8d5c-b8f81df00e80/resources/517b36a6-9ca2-4e7b-9748-3af25f5cd4fd
```

# [C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationexcelresource-from-educationassignment-e3-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [CLI](#tab/cli)
[!INCLUDE [sample-code](../includes/snippets/cli/get-educationexcelresource-from-educationassignment-e3-cli-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-educationexcelresource-from-educationassignment-e3-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-educationexcelresource-from-educationassignment-e3-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationexcelresource-from-educationassignment-e3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [PHP](#tab/php)
[!INCLUDE [sample-code](../includes/snippets/php/get-educationexcelresource-from-educationassignment-e3-php-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/get-educationexcelresource-from-educationassignment-e3-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [Python](#tab/python)
[!INCLUDE [sample-code](../includes/snippets/python/get-educationexcelresource-from-educationassignment-e3-python-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### Response
The following example shows the response.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationExcelResource"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#education/classes('72a7baec-c3e9-4213-a850-f62de0adad5f')/assignments('1618dfb0-3ff2-4edf-8d5c-b8f81df00e80')/resources/$entity",
    "distributeForStudentWork": false,
    "id": "517b36a6-9ca2-4e7b-9748-3af25f5cd4fd",
    "resource": {
        "@odata.type": "#microsoft.graph.educationExcelResource",
        "displayName": "Graph Doc pages.xlsx",
        "createdDateTime": "2021-09-13T15:50:49.7107759Z",
        "lastModifiedDateTime": "2021-09-13T15:50:49.7107759Z",
        "fileUrl": "https://graph.microsoft.com/beta/drives/b!OPmUsPgnBUiMIXMxWcj3neC1xck6I5NIsnFxfrLdmXoOOmEQNO79QpIMPdOmY3nf/items/01QTY63RIR7PSV4JJSFJHKNPUVUWGPW4O2",
        "createdBy": {
            "application": null,
            "device": null,
            "user": {
                "id": "f3a5344e-dbde-48b0-be24-b5b62a243836",
                "displayName": null
            }
        },
        "lastModifiedBy": {
            "application": null,
            "device": null,
            "user": {
                "id": "f3a5344e-dbde-48b0-be24-b5b62a243836",
                "displayName": null
            }
        }
    }
}
```

### Example 4: Get an educationPowerPointResource
#### Request
The following example shows a request.

# [HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["72a7baec-c3e9-4213-a850-f62de0adad5f","1618dfb0-3ff2-4edf-8d5c-b8f81df00e80","3cb7968b-082f-4756-bdfb-782b4538cc0a"], 
  "name": "get_educationpowerpointresource_from_educationassignment_e4"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/education/classes/72a7baec-c3e9-4213-a850-f62de0adad5f/assignments/1618dfb0-3ff2-4edf-8d5c-b8f81df00e80/resources/3cb7968b-082f-4756-bdfb-782b4538cc0a
```

# [C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationpowerpointresource-from-educationassignment-e4-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [CLI](#tab/cli)
[!INCLUDE [sample-code](../includes/snippets/cli/get-educationpowerpointresource-from-educationassignment-e4-cli-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-educationpowerpointresource-from-educationassignment-e4-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-educationpowerpointresource-from-educationassignment-e4-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationpowerpointresource-from-educationassignment-e4-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [PHP](#tab/php)
[!INCLUDE [sample-code](../includes/snippets/php/get-educationpowerpointresource-from-educationassignment-e4-php-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/get-educationpowerpointresource-from-educationassignment-e4-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [Python](#tab/python)
[!INCLUDE [sample-code](../includes/snippets/python/get-educationpowerpointresource-from-educationassignment-e4-python-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### Response
The following example shows the response.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationPowerPointResource"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#education/classes('72a7baec-c3e9-4213-a850-f62de0adad5f')/assignments('1618dfb0-3ff2-4edf-8d5c-b8f81df00e80')/resources/$entity",
    "distributeForStudentWork": false,
    "id": "3cb7968b-082f-4756-bdfb-782b4538cc0a",
    "resource": {
        "@odata.type": "#microsoft.graph.educationPowerPointResource",
        "displayName": "state diagram.pptx",
        "createdDateTime": "2021-09-13T15:50:58.5428117Z",
        "lastModifiedDateTime": "2021-09-13T15:50:58.5428117Z",
        "fileUrl": "https://graph.microsoft.com/beta/drives/b!OPmUsPgnBUiMIXMxWcj3neC1xck6I5NIsnFxfrLdmXoOOmEQNO79QpIMPdOmY3nf/items/01QTY63RN327OXRN6EVFE2Q5FRJZTN5EOJ",
        "createdBy": {
            "application": null,
            "device": null,
            "user": {
                "id": "f3a5344e-dbde-48b0-be24-b5b62a243836",
                "displayName": null
            }
        },
        "lastModifiedBy": {
            "application": null,
            "device": null,
            "user": {
                "id": "f3a5344e-dbde-48b0-be24-b5b62a243836",
                "displayName": null
            }
        }
    }
}
```

### Example 5: Get an educationFileResource
#### Request
The following example shows a request.

# [HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["72a7baec-c3e9-4213-a850-f62de0adad5f","1618dfb0-3ff2-4edf-8d5c-b8f81df00e80","a7a2fec0-2a26-47bf-8d40-2319c0afb1f4"], 
  "name": "get_educationfileresource_from_educationassignment_e5"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/education/classes/72a7baec-c3e9-4213-a850-f62de0adad5f/assignments/1618dfb0-3ff2-4edf-8d5c-b8f81df00e80/resources/a7a2fec0-2a26-47bf-8d40-2319c0afb1f4
```

# [C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationfileresource-from-educationassignment-e5-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [CLI](#tab/cli)
[!INCLUDE [sample-code](../includes/snippets/cli/get-educationfileresource-from-educationassignment-e5-cli-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-educationfileresource-from-educationassignment-e5-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-educationfileresource-from-educationassignment-e5-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationfileresource-from-educationassignment-e5-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [PHP](#tab/php)
[!INCLUDE [sample-code](../includes/snippets/php/get-educationfileresource-from-educationassignment-e5-php-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/get-educationfileresource-from-educationassignment-e5-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [Python](#tab/python)
[!INCLUDE [sample-code](../includes/snippets/python/get-educationfileresource-from-educationassignment-e5-python-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### Response
The following example shows the response.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationFileResource"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#education/classes('72a7baec-c3e9-4213-a850-f62de0adad5f')/assignments('1618dfb0-3ff2-4edf-8d5c-b8f81df00e80')/resources/$entity",
    "distributeForStudentWork": false,
    "id": "a7a2fec0-2a26-47bf-8d40-2319c0afb1f4",
    "resource": {
        "@odata.type": "#microsoft.graph.educationFileResource",
        "displayName": "factura.pdf",
        "createdDateTime": "2021-09-13T15:51:24.4663092Z",
        "lastModifiedDateTime": "2021-09-13T15:51:24.4663092Z",
        "fileUrl": "https://graph.microsoft.com/beta/drives/b!OPmUsPgnBUiMIXMxWcj3neC1xck6I5NIsnFxfrLdmXoOOmEQNO79QpIMPdOmY3nf/items/01QTY63RPHKSP6THE4ORD2RQAR6MQLF26G",
        "createdBy": {
            "application": null,
            "device": null,
            "user": {
                "id": "f3a5344e-dbde-48b0-be24-b5b62a243836",
                "displayName": null
            }
        },
        "lastModifiedBy": {
            "application": null,
            "device": null,
            "user": {
                "id": "f3a5344e-dbde-48b0-be24-b5b62a243836",
                "displayName": null
            }
        }
    }
}
```

### Example 6: Get an educationMediaResource
#### Request
The following example shows a request.

# [HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["72a7baec-c3e9-4213-a850-f62de0adad5f","1618dfb0-3ff2-4edf-8d5c-b8f81df00e80","f3687fc5-908b-4006-8040-dbba9e04023c"], 
  "name": "get_educationmediaresource_from_educationassignment_e6"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/education/classes/72a7baec-c3e9-4213-a850-f62de0adad5f/assignments/1618dfb0-3ff2-4edf-8d5c-b8f81df00e80/resources/f3687fc5-908b-4006-8040-dbba9e04023c
```

# [C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationmediaresource-from-educationassignment-e6-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [CLI](#tab/cli)
[!INCLUDE [sample-code](../includes/snippets/cli/get-educationmediaresource-from-educationassignment-e6-cli-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-educationmediaresource-from-educationassignment-e6-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-educationmediaresource-from-educationassignment-e6-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationmediaresource-from-educationassignment-e6-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [PHP](#tab/php)
[!INCLUDE [sample-code](../includes/snippets/php/get-educationmediaresource-from-educationassignment-e6-php-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/get-educationmediaresource-from-educationassignment-e6-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [Python](#tab/python)
[!INCLUDE [sample-code](../includes/snippets/python/get-educationmediaresource-from-educationassignment-e6-python-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### Response
The following example shows the response.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationMediaResource"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#education/classes('72a7baec-c3e9-4213-a850-f62de0adad5f')/assignments('1618dfb0-3ff2-4edf-8d5c-b8f81df00e80')/resources/$entity",
    "distributeForStudentWork": false,
    "id": "f3687fc5-908b-4006-8040-dbba9e04023c",
    "resource": {
        "@odata.type": "#microsoft.graph.educationMediaResource",
        "displayName": "homework example.PNG",
        "createdDateTime": "2021-09-23T18:30:16.314644Z",
        "lastModifiedDateTime": "2021-09-23T18:30:16.314644Z",
        "fileUrl": "https://graph.microsoft.com/beta/drives/b!OPmUsPgnBUiMIXMxWcj3neC1xck6I5NIsnFxfrLdmXoOOmEQNO79QpIMPdOmY3nf/items/01QTY63RMUWOKAGSJZ6BHINJVKNMOOJABF",
        "createdBy": {
            "application": null,
            "device": null,
            "user": {
                "id": "f3a5344e-dbde-48b0-be24-b5b62a243836",
                "displayName": null
            }
        },
        "lastModifiedBy": {
            "application": null,
            "device": null,
            "user": {
                "id": "f3a5344e-dbde-48b0-be24-b5b62a243836",
                "displayName": null
            }
        }
    }
}
```

### Example 7: Get an educationSpeakerProgressResource

The following example shows how to get an [educationSpeakerProgressResource](../resources/educationspeakerprogressresource.md) assignment resource.

#### Request

The following example shows a request.

<!-- {
  "blockType": "request",
  "name": "specific_educationSpeakerProgressResource"
}
-->
``` http
GET https://graph.microsoft.com/beta/education/classes/37d99af7-cfc5-4e3b-8566-f7d40e4a2070/assignments/fe9c8d6f-baad-4b5e-b9d5-e2bb33e4ed19/resources/af98a1e1-3393-4ee0-8bcc-8b5bb4598d1c
```

### Response

The following example shows the response.
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSpeakerProgressResource"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#education/classes('37d99af7-cfc5-4e3b-8566-f7d40e4a2070')/assignments('fe9c8d6f-baad-4b5e-b9d5-e2bb33e4ed19')/resources/$entity",
  "distributeForStudentWork": true,
  "id": "af98a1e1-3393-4ee0-8bcc-8b5bb4598d1c",
  "resource": {
    "@odata.type": "#microsoft.graph.educationSpeakerProgressResource",
    "displayName": "speakerProgressTestResource",
    "createdDateTime": "2025-03-17T16:26:03.5530234Z",
    "lastModifiedDateTime": "2025-03-17T16:26:03.5530384Z",
    "recordingTimeLimitInMinutes": 5,
    "showRehearsalReportToStudentBeforeMediaUpload": true,
    "maxRecordingAttempts": 1,
    "isVideoRequired": true,
    "isAiFeedbackEnabled": true,
    "presentationTitle": "speakerProgressTestResource",
    "spokenLanguageLocale": "en-US",
    "createdBy": {
      "application": null,
      "device": null,
      "user": {
        "id": "fffafb29-e8bc-4de3-8106-be76ed2ad499",
        "displayName": null
      }
    },
    "lastModifiedBy": {
      "application": null,
      "device": null,
      "user": {
        "id": "fffafb29-e8bc-4de3-8106-be76ed2ad499",
        "displayName": null
      }
    },
    "speakerCoachSettings": {
      "deliverySettings": {
        "isPaceEnabled": false,
        "areFillerWordsEnabled": false,
        "isPitchEnabled": false,
        "isPronunciationEnabled": true
      },
      "contentSettings": {
        "isInclusivenessEnabled": false,
        "isRepetitiveLanguageEnabled": false
      },
      "audienceEngagementSettings": {
        "isBodyLanguageEnabled": false
      }
    },
    "aiFeedbackCriteria": {
      "speechType": "informative",
      "aiFeedbackSettings": {
        "deliverySettings": {
          "isLanguageUseEnabled": false,
          "areRhetoricalTechniquesEnabled": false,
          "isStyleEnabled": true
        },
        "contentSettings": {
          "isSpeechOrganizationEnabled": false,
          "isMessageClarityEnabled": false,
          "isQualityOfInformationEnabled": false
        },
        "audienceEngagementSettings": {
          "areEngagementStrategiesEnabled": false,
          "isEmotionalAndIntellectualAppealEnabled": false,
          "isCallToActionEnabled": false
        }
      }
    }
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get educationAssignmentResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
