
```Cs

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var message = await graphClient.Me.Messages["AAMkAGVmMDEz"]
	.Request()
	.Select( e => new {
			 e.InternetMessageHeaders 
			 })
	.GetAsync();

```