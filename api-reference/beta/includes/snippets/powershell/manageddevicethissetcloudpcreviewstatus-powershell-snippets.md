---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershell

Import-Module Microsoft.Graph.Beta.DeviceManagement

$params = @{
	reviewStatus = @{
		inReview = $true
		userAccessLevel = "restricted"
		azureStorageAccountId = "/subscriptions/f68bd846-16ad-4b51-a7c6-c84944a3367c/resourceGroups/Review/providers/Microsoft.Storage/storageAccounts/snapshotsUnderReview"
	}
}

Set-MgBetaDeviceManagementManagedDeviceCloudPcReviewStatus -ManagedDeviceId $managedDeviceId -BodyParameter $params

```