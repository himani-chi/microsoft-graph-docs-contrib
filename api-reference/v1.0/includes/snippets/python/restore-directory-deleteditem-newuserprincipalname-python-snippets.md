---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

# Code snippets are only available for the latest version. Current version is 1.x
from msgraph import GraphServiceClient
from msgraph.generated.directory.deleteditems.item.restore.restore_post_request_body import RestorePostRequestBody
# To initialize your graph_client, see https://learn.microsoft.com/en-us/graph/sdks/create-client?from=snippets&tabs=python
request_body = RestorePostRequestBody(
	additional_data = {
			"new_user_principal_name" : "johndoe@contoso.com",
	}
)

result = await graph_client.directory.deleted_items.by_directory_object_id('directoryObject-id').restore.post(request_body)


```