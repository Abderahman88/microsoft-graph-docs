---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var chatMessage = await graphClient.Teams["{team-id}"].Channels["{channel-id}"].Messages["{chatMessage-id}"]
	.Request()
	.Top(2)
	.GetAsync();

```