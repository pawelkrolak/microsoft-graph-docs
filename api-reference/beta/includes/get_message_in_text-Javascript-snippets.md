
```Javascript

const options = {
	authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/messages/AAMkAGI1AAAoZCfHAAA=/')
	.version('beta')
	.header('Prefer','outlook.body-content-type="text"')
	.select('subject,body,bodyPreview,uniqueBody')
	.get();

```