---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

<?php
use Microsoft\Graph\Beta\GraphServiceClient;


$graphServiceClient = new GraphServiceClient($tokenRequestContext, $scopes);


$result = $graphServiceClient->storage()->fileStorage()->containers()->byFileStorageContainerId('fileStorageContainer-id')->sharePointGroups()->bySharePointGroupId('sharePointGroup-id')->members()->bySharePointGroupMemberId('sharePointGroupMember-id')->get()->wait();

```