---
description: "Automatically generated file. DO NOT MODIFY"
---

```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewAuthorizationPolicy()
requestBody.SetPermissionGrantPolicyIdsAssignedToDefaultUserRole( []String {
	"managePermissionGrantsForSelf.microsoft-user-default-low",
}
options := &msgraphsdk.AuthorizationPolicyRequestBuilderPatchOptions{
	Body: requestBody,
}
authorizationPolicyId := "authorizationPolicy-id"
graphClient.Policies().AuthorizationPolicyById(&authorizationPolicyId).Patch(options)


```