---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

<?php
use Microsoft\Graph\Beta\GraphServiceClient;
use Microsoft\Graph\Beta\Generated\Models\DeviceTemplate;


$graphServiceClient = new GraphServiceClient($tokenRequestContext, $scopes);

$requestBody = new DeviceTemplate();
$requestBody->setMutualTlsOauthConfigurationId('00001111-aaaa-2222-bbbb-3333cccc4444');
$requestBody->setMutualTlsOauthConfigurationTenantId('00001111-aaaa-2222-bbbb-3333cccc4445');
$requestBody->setDeviceAuthority('Lakeshore Retail');
$requestBody->setManufacturer('Tailwind Traders');
$requestBody->setModel('DeepFreezerModelAB');
$requestBody->setOperatingSystem('WindowsIoT');
$additionalData = [
	'owners@odata.bind' => [
'https://graph.microsoft.com/beta/users/aaaaaaaa-bbbb-cccc-1111-222222222222', ],
];
$requestBody->setAdditionalData($additionalData);

$result = $graphServiceClient->directory()->templates()->deviceTemplates()->post($requestBody)->wait();

```