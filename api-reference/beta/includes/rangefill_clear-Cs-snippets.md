
```Cs

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Drive.Items["{id}"].Workbook.Names["{name}"]
	.Range().Format.Fill
	.Clear()
	.Request()
	.PostAsync()

```