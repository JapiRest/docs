# WikiHow

## Search

```shell
curl "https://japi.rest/mywaifulist/v1/waifu/sylvie-4" \
  -H "Authorization: {API KEY}"
```

```javascript
const fetch = require('node-fetch'); // NodeJS users
const waifuName = 'sylvie-4';
const data = fetch(`https://japi.rest/mywaifulist/v1/waifu/${waifuName}`, {
  headers: { "Authorization": "{API KEY}" }
}).then(res => res.json())

console.log(data);
```

> The above command returns JSON structured like this:

```json
{
  "cache_expiry": 3600,
  "cached": false,
  "data": {
    "name": "Sylvie",
    "description": "Sylvie is an artist in the example Ren Py visual novel, The Question.",
    "image": "https://thicc.mywaifulist.moe/waifus/26329/ea3bf9950e1e70afc1fa0088ad3aad5cf9817b113c9e9c6081c4fc246b5aeeec_thumb.png",
    "url": "https://mywaifulist.moe/waifu/sylvie-4"
  }
}
```

This endpoint retrieves information from mywaifulist using the waifu name.

### HTTP Request

`GET https://japi.rest/mywaifulist/v1/waifu/:name`

### Path Parameters

Parameter | Required | Description
--------- | -------- | -----------
name      | true     | The waifu name

## Random

```shell
curl "https://japi.rest/mywaifulist/v1/random" \
  -H "Authorization: {API KEY}"
```

```javascript
const fetch = require('node-fetch'); // NodeJS users
const data = fetch(`https://japi.rest/mywaifulist/v1/random`, {
  headers: { "Authorization": "{API KEY}" }
}).then(res => res.json())

console.log(data);
```

> The above command returns JSON structured like this:

```json
{
  "cache_expiry": 3600,
  "cached": false,
  "data": {
    "name": "Sylvie",
    "description": "Sylvie is an artist in the example Ren Py visual novel, The Question.",
    "image": "https://thicc.mywaifulist.moe/waifus/26329/ea3bf9950e1e70afc1fa0088ad3aad5cf9817b113c9e9c6081c4fc246b5aeeec_thumb.png",
    "url": "https://mywaifulist.moe/waifu/sylvie-4"
  },
  "url": "https://japi.rest/mywaifulist/v1/waifu/sylvie-4"
}
```

This endpoint retrieves a article's information.

### HTTP Request

`GET https://japi.rest/mywaifulist/v1/random`