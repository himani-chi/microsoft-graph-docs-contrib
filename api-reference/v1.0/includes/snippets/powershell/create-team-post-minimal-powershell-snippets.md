---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershell

Import-Module Microsoft.Graph.Teams

$params = @{
	"template@odata.bind" = "https://graph.microsoft.com/v1.0/teamsTemplates('standard')"
	displayName = "My Sample Team"
	description = "My sample team’s description"
	firstChannelName = "My first channel of the sample team"
	members = @(
		@{
			"@odata.type" = "#microsoft.graph.aadUserConversationMember"
			roles = @(
			"owner"
		)
		"user@odata.bind" = "https://graph.microsoft.com/v1.0/users('0040b377-61d8-43db-94f5-81374122dc7e')"
	}
)
}

New-MgTeam -BodyParameter $params

```