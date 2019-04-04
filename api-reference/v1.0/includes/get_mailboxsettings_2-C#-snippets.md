
```CS

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var mailboxSettings = await graphClient.Me
	.Request()
	.Select("automaticRepliesSetting")
	.GetAsync();

var automaticRepliesSetting = mailboxSettings.AutomaticRepliesSetting;

```