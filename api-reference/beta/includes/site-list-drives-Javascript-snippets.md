
```Javascript

const options = {
	authProvider,
};

const client = Client.init(options);

let res = await client.api('/sites/{siteId}/drives')
	.version('beta')
	.get();

```