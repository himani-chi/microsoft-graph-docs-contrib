---
description: "Automatically generated file. DO NOT MODIFY"
---

```go


// Code snippets are only available for the latest major version. Current major version is $v1.*

// Dependencies
import (
	  "context"
	  msgraphsdk "github.com/microsoftgraph/msgraph-sdk-go"
	  graphsites "github.com/microsoftgraph/msgraph-sdk-go/sites"
	  //other-imports
)


requestToken := "latest"

requestParameters := &graphsites.ItemListsItemItemsDeltaRequestBuilderGetQueryParameters{
	Token: &requestToken,
}
configuration := &graphsites.ItemListsItemItemsDeltaRequestBuilderGetRequestConfiguration{
	QueryParameters: requestParameters,
}

// To initialize your graphClient, see https://learn.microsoft.com/en-us/graph/sdks/create-client?from=snippets&tabs=go
delta, err := graphClient.Sites().BySiteId("site-id").Lists().ByListId("list-id").Items().Delta().GetAsDeltaGetResponse(context.Background(), configuration)


```