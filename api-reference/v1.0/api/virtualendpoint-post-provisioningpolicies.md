---
title: "Create cloudPcProvisioningPolicy"
description: "Create a new Cloud PC provisioning policy object."
author: "AshleyYangSZ"
ms.localizationpriority: medium
ms.subservice: "cloud-pc"
doc_type: apiPageType
ms.date: 09/27/2024
---

# Create cloudPcProvisioningPolicy

Namespace: microsoft.graph

Create a new [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) object.

[!INCLUDE [national-cloud-support](../../includes/global-only.md)]

## Permissions

Choose the permission or permissions marked as least privileged for this API. Use a higher privileged permission or permissions [only if your app requires it](/graph/permissions-overview#best-practices-for-using-microsoft-graph-permissions). For details about delegated and application permissions, see [Permission types](/graph/permissions-overview#permission-types). To learn more about these permissions, see the [permissions reference](/graph/permissions-reference).

<!-- { "blockType": "permissions", "name": "virtualendpoint_post_provisioningpolicies" } -->
[!INCLUDE [permissions-table](../includes/permissions/virtualendpoint-post-provisioningpolicies-permissions.md)]

## HTTP request

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /deviceManagement/virtualEndpoint/provisioningPolicies
```

## Request headers

| Name          | Description                |
| :------------ | :------------------------  |
|Authorization|Bearer {token}. Required. Learn more about [authentication and authorization](/graph/auth/auth-concepts).|
| Content-Type  | application/json. Required.|

## Request body

In the request body, supply a JSON representation of the [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) object.

The following table lists the properties that are required when you create the [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md).

|Property|Type|Description|
|:---|:---|:---|
|cloudPcNamingTemplate|String|The template used to name Cloud PCs provisioned using this policy. The template can contain custom text and replacement tokens, including `%USERNAME:x%` and `%RAND:x%`, which represent the user's name and a randomly generated number, respectively. For example, `CPC-%USERNAME:4%-%RAND:5%` means that the name of the Cloud PC starts with `CPC-`, followed by a four-character username, a `-` character, and then five random characters. The total length of the text generated by the template can't exceed 15 characters. Supports `$filter`, `$select`, and `$orderby`.|
|description|String|The provisioning policy description. Supports `$filter`, `$select`, and `$orderBy`. |
|displayName|String|The display name for the provisioning policy.|
|domainJoinConfigurations|[cloudPcDomainJoinConfiguration](../resources/cloudpcdomainjoinconfiguration.md) collection|Specifies a list ordered by priority on how Cloud PCs join Microsoft Entra ID.|
|enableSingleSignOn|Boolean|`True` if the provisioned Cloud PC can be accessed by single sign-on. `False` indicates that the provisioned Cloud PC doesn't support this feature. The default value is `false`. Windows 365 users can use single sign-on to authenticate to Microsoft Entra ID with passwordless options (for example, FIDO keys) to access their Cloud PC. Optional.|
|imageDisplayName|String|The display name for the OS image you’re provisioning.|
|imageId|String|The ID of the operating system image you want to provision on Cloud PCs. The format for a gallery type image is: {publisher_offer_sku}. Supported values for each of the parameters are as follows:<ul><li>publisher: `Microsoftwindowsdesktop`.</li> <li>offer: `windows-ent-cpc`.</li> <li>sku: `21h1-ent-cpc-m365`, `21h1-ent-cpc-os`, `20h2-ent-cpc-m365`, `20h2-ent-cpc-os`, `20h1-ent-cpc-m365`, `20h1-ent-cpc-os`, `19h2-ent-cpc-m365`, and `19h2-ent-cpc-os`.</li></ul>|
|imageType|[cloudPcProvisioningPolicyImageType](../resources/cloudpcprovisioningpolicy.md#cloudpcprovisioningpolicyimagetype-values)|The type of OS image (custom or gallery) you want to provision on Cloud PCs. Possible values are: `gallery`, `custom`, `unknownFutureValue`.|
|microsoftManagedDesktop|[microsoftManagedDesktop](../resources/microsoftmanageddesktop.md)|The specific settings to **microsoftManagedDesktop** that enables Microsoft Managed Desktop customers to get device managed experience for Cloud PC. To enable **microsoftManagedDesktop** to provide more value, an admin needs to specify certain settings in it. Supports `$filter`, `$select`, and `$orderBy`.|
|provisioningType|[cloudPcProvisioningType](../resources/cloudpcprovisioningpolicy.md#cloudpcprovisioningtype-values)|Specifies the type of license used when provisioning Cloud PCs using this policy. By default, the license type is `dedicated` if the **provisioningType** isn't specified when you create the **cloudPcProvisioningPolicy**. You can't change this property after the **cloudPcProvisioningPolicy** was created. Possible values are: `dedicated`, `shared`, `unknownFutureValue`.|
|windowsSetting|[cloudPcWindowsSetting](../resources/cloudpcwindowssetting.md)|Indicates a specific Windows setting to configure during the creation of Cloud PCs for this provisioning policy. Supports `$select`. |

## Response

If successful, this method returns a `201 Created` response code and a [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) object in the response body.

## Examples

### Request

The following example shows a request.

# [HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_cloudpcprovisioningpolicy_from_cloudpcprovisioningpolicy"
}
-->

``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/virtualEndpoint/provisioningPolicies
Content-Type: application/json

{
    "@odata.type": "#microsoft.graph.cloudPcProvisioningPolicy",
    "description": "Description value",
    "displayName": "Display Name value",
    "domainJoinConfigurations": [
      {
        "onPremisesConnectionId": "16ee6c71-fc10-438b-88ac-daa1ccafffff",
        "domainJoinType": "hybridAzureADJoin"
      },
      {
        "onPremisesConnectionId": "26e16c71-f210-438b-88ac-d481ccafffff",
        "domainJoinType": "hybridAzureADJoin"
      }
    ],
    "id": "1d164206-bf41-4fd2-8424-a3192d39ffff",
    "enableSingleSignOn": true,
    "imageDisplayName": "Windows-10 19h1-evd",
    "imageId": "MicrosoftWindowsDesktop_Windows-10_19h1-evd",
    "imageType":"gallery",
    "windowsSetting": {
        "locale": "en-US"
    },
    "provisioningType": "dedicated"
}
```

# [C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-cloudpcprovisioningpolicy-from-cloudpcprovisioningpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [CLI](#tab/cli)
[!INCLUDE [sample-code](../includes/snippets/cli/create-cloudpcprovisioningpolicy-from-cloudpcprovisioningpolicy-cli-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/create-cloudpcprovisioningpolicy-from-cloudpcprovisioningpolicy-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-cloudpcprovisioningpolicy-from-cloudpcprovisioningpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-cloudpcprovisioningpolicy-from-cloudpcprovisioningpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [PHP](#tab/php)
[!INCLUDE [sample-code](../includes/snippets/php/create-cloudpcprovisioningpolicy-from-cloudpcprovisioningpolicy-php-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/create-cloudpcprovisioningpolicy-from-cloudpcprovisioningpolicy-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [Python](#tab/python)
[!INCLUDE [sample-code](../includes/snippets/python/create-cloudpcprovisioningpolicy-from-cloudpcprovisioningpolicy-python-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### Response

The following example shows the response.

> **Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.cloudPcProvisioningPolicy"
}
-->

``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.cloudPcProvisioningPolicy",
  "description": "Description value",
  "displayName": "Display Name value",
  "domainJoinConfigurations": [
    {
      "onPremisesConnectionId": "16ee6c71-fc10-438b-88ac-daa1ccafffff",
      "domainJoinType": "hybridAzureADJoin"
    },
    {
      "onPremisesConnectionId": "26e16c71-f210-438b-88ac-d481ccafffff",
      "domainJoinType": "hybridAzureADJoin"
    }
  ],
   "microsoftManagedDesktop": {
      "managedType": "notManaged",
      "profile": null
  },
  "autopatch": {
      "autopatchGroupId": null
  },
  "enableSingleSignOn": true,
  "id": "1d164206-bf41-4fd2-8424-a3192d39ffff",
  "imageDisplayName": "Windows-10 19h1-evd",
  "imageId": "MicrosoftWindowsDesktop_Windows-10_19h1-evd",
  "imageType":"gallery",
  "windowsSetting": {
      "locale": "en-US"
  },
  "provisioningType": "dedicated"
}
```
