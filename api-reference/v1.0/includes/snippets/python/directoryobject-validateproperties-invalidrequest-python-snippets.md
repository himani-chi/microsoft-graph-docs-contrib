---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

# Code snippets are only available for the latest version. Current version is 1.x
from msgraph import GraphServiceClient
from msgraph.generated.directoryobjects.validate_properties.validate_properties_post_request_body import ValidatePropertiesPostRequestBody
# To initialize your graph_client, see https://learn.microsoft.com/en-us/graph/sdks/create-client?from=snippets&tabs=python
request_body = ValidatePropertiesPostRequestBody(
	entity_type = "Group",
	display_name = "test",
	mail_nickname = "test",
	on_behalf_of_user_id = UUID("onBehalfOfUserId-value"),
)

await graph_client.directory_objects.validate_properties.post(request_body)


```