
```Cs

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var secureScoreControlProfile = new SecureScoreControlProfile
{
	ControlStateUpdates = "controlStateUpdates-value",
};

await graphClient.Security.SecureScoreControlProfiles["AdminMFA"]
	.Request()
	.UpdateAsync(secureScoreControlProfile);

```