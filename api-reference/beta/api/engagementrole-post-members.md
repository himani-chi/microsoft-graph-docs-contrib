---
title: "Create engagementRoleMember"
description: "Create a new engagementRoleMember object."
author: "richafnu"
ms.date: 03/27/2025
ms.localizationpriority: medium
ms.subservice: "viva-engage"
doc_type: apiPageType
---

# Create engagementRoleMember

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Assign a Viva Engage role to a user.

## Permissions

Choose the permission or permissions marked as least privileged for this API. Use a higher privileged permission or permissions [only if your app requires it](/graph/permissions-overview#best-practices-for-using-microsoft-graph-permissions). For details about delegated and application permissions, see [Permission types](/graph/permissions-overview#permission-types). To learn more about these permissions, see the [permissions reference](/graph/permissions-reference).

<!-- { "blockType": "permissions", "name": "engagementrole_post_members" } -->
[!INCLUDE [permissions-table](../includes/permissions/engagementrole-post-members-permissions.md)]

## HTTP request

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /employeeExperience/roles/{engagementRoleId}/members
```

## Request headers

|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required. Learn more about [authentication and authorization](/graph/auth/auth-concepts).|
|Content-Type|application/json. Required.|

## Request body

In the request body, supply a JSON representation of the [engagementRoleMember](../resources/engagementrolemember.md) object.

You can specify the following properties when creating an **engagementRoleMember**.

|Property|Type|Description|
|:---|:---|:---|
|userId|String|The Microsoft Entra ID of the user who has the role assigned.|
|createdDateTime|DateTimeOffset|The timestamp when the role was assigned to the user.|

## Response

If successful, this method returns a `201 Created` response code and an [engagementRoleMember](../resources/engagementrolemember.md) object in the response body.

## Examples

### Request

The following example shows a request.
<!-- {
  "blockType": "request",
  "name": "create_engagementrolemember_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/employeeExperience/roles/{engagementRoleId}/members
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.engagementrolemember",
  "userId": "String"
}
```

### Response

The following example shows the response.
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.engagementrolemember"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.engagementRoleMember",
  "id": "a40473a5-0fb4-a250-e029-f6fe33d07733",
  "userId": "String",
  "createdDateTime": "String (timestamp)"
}
```

