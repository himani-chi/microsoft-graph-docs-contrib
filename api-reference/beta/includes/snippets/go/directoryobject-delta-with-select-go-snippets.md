---
description: "Automatically generated file. DO NOT MODIFY"
---

```go


// Code snippets are only available for the latest major version. Current major version is $v0.*

// Dependencies
import (
	  "context"
	  msgraphsdk "github.com/microsoftgraph/msgraph-beta-sdk-go"
	  graphdirectoryobjects "github.com/microsoftgraph/msgraph-beta-sdk-go/directoryobjects"
	  //other-imports
)


requestFilter := "isof('microsoft.graph.user') or isof('microsoft.graph.group')"

requestParameters := &graphdirectoryobjects.DirectoryObjectsDeltaRequestBuilderGetQueryParameters{
	Filter: &requestFilter,
	Select: [] string {"microsoft.graph.user/surname","microsoft.graph.group/displayName"},
}
configuration := &graphdirectoryobjects.DirectoryObjectsDeltaRequestBuilderGetRequestConfiguration{
	QueryParameters: requestParameters,
}

// To initialize your graphClient, see https://learn.microsoft.com/en-us/graph/sdks/create-client?from=snippets&tabs=go
delta, err := graphClient.DirectoryObjects().Delta().GetAsDeltaGetResponse(context.Background(), configuration)


```