---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

<?php
use Microsoft\Graph\Beta\GraphServiceClient;


$graphServiceClient = new GraphServiceClient($tokenRequestContext, $scopes);


$result = $graphServiceClient->reports()->serviceActivity()->getMetricsForConditionalAccessBlockedSignInWithInclusiveIntervalStartDateTimeWithExclusiveIntervalEndDateTime(new \DateTime('{exclusiveIntervalEndDateTime}'),new \DateTime('{inclusiveIntervalStartDateTime}'))->get()->wait();

```