---
description: "Automatically generated file. DO NOT MODIFY"
---

```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ChannelCollectionPage channels = graphClient.teams("{id}").channels()
	.buildRequest()
	.filter("membershipType eq 'private'")
	.get();

```