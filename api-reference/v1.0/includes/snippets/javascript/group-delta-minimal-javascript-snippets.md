---
description: "Automatically generated file. DO NOT MODIFY"
---

```javascript

const options = {
	authProvider,
};

const client = Client.init(options);

let delta = await client.api('/groups/delta')
	.header('Prefer','return=minimal')
	.select('displayName,description,mailNickname')
	.get();

```