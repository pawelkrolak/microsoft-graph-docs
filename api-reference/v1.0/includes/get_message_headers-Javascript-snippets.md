
```Javascript

const options = {
	authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/messages/AAMkADhAAAW-VPeAAA=/')
	.select('internetMessageHeaders')
	.get();

```