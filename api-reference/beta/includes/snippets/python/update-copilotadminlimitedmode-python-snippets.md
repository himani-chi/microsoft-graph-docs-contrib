---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

# Code snippets are only available for the latest version. Current version is 1.x
from msgraph_beta import GraphServiceClient
from msgraph_beta.generated.models.copilot_admin_limited_mode import CopilotAdminLimitedMode
# To initialize your graph_client, see https://learn.microsoft.com/en-us/graph/sdks/create-client?from=snippets&tabs=python
request_body = CopilotAdminLimitedMode(
	odata_type = "#microsoft.graph.copilotAdminLimitedMode",
	is_enabled_for_group = True,
	group_id = "4c563cdf-0efa-44c5-a384-dbf57db277df",
)

result = await graph_client.copilot.admin.settings.limited_mode.patch(request_body)


```