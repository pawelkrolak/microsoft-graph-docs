
```Javascript

const options = {
	authProvider,
};

const client = Client.init(options);

let res = await client.api('/groups/{id}/threads/{id}/posts/{id}/attachments')
	.version('beta')
	.get();

```