---
description: "Automatically generated file. DO NOT MODIFY"
---

```java

// Code snippets are only available for the latest version. Current version is 6.x

GraphServiceClient graphClient = new GraphServiceClient(requestAdapter);

var result = graphClient.education().classes().byEducationClassId("{educationClass-id}").getRecentlyModifiedSubmissions().get(requestConfiguration -> {
	requestConfiguration.queryParameters.filter = "lastModifiedDateTime lt 2025-04-29T15:48:31.3785886Z";
});


```