---
description: "Automatically generated file. DO NOT MODIFY"
---

```javascript

const options = {
	authProvider,
};

const client = Client.init(options);

let hostedContents = await client.api('/chats/{id}/messages/{id}/hostedContents')
	.version('beta')
	.get();

```