---
description: "Automatically generated file. DO NOT MODIFY"
---

```javascript

const options = {
	authProvider,
};

const client = Client.init(options);

await client.api('/me/events/{id}/attachments/{id}')
	.version('beta')
	.delete();

```