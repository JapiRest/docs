# Discord

## Get User

```shell
curl "https://japi.rest/discord/v1/user?id=:userId" \
  -H "Authorization: Bearer {API KEY}"
```

```javascript
const data = fetch("https://japi.rest/discord/v1/user?id=:userId")

let api = kittn.authorize('Bearer {API KEY}');
let kittens = api.kittens.get();
```

> Make sure to replaxe {API KEY} with your actual API key.

> The above command returns JSON structured like this:

```json
{
  "data": {
    "id": ":userId",
    "username": ":username",
    "discriminator": ":discriminator",
    "avatar": ":avatar",
    "created_at": ":created_at",
    "bio": ":bio",
    "default_avatar": ":default_avatar",
  }
}
```

This endpoint retrieves a user's information.

### HTTP Request

`GET https://japi.rest/discord/v1/user?id=:userId`

### Query Parameters

Parameter | Required | Description
--------- | ------- | -----------
id | true | The user's ID.
