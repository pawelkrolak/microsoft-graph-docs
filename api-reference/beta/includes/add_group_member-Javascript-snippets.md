
```Javascript

const options = {
	authProvider,
};

const client = Client.init(options);

const directoryObject = {
  @odata.id: "https://graph.microsoft.com/beta/directoryObjects/{id}"
};

let res = await client.api('/groups/{id}/members/$ref')
	.version('beta')
	.post({directoryObject : directoryObject});

```