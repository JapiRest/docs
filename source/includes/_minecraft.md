# Minecraft

## UUID from MC Username

```shell
curl "https://japi.rest/minecraft/v1/username/DanPlayz" \
  -H "Authorization: {API KEY}"
```

```javascript
const username = 'DanPlayz';
const data = fetch(`https://japi.rest/minecraft/v1/username/${username}`, {
  headers: { "Authorization": "{API KEY}" }
}).then(res => res.json()).then(data => console.log(data));
```

> The above command returns JSON structured like this:

```json
{
  "cache_expiry": 10800,
  "cached": false,
  "data": {
    "name": "DanPlayz",
    "id": "41f9049d58204631b8aa18f8397ba5c1"
  }
}
```

This endpoint retrieves the uuid for a username from mojang.

### HTTP Request

`GET https://japi.rest/minecraft/v1/username/:username`

### Path Parameters

Parameter | Required | Description
----------|----------|----------------------------------------------
username  | true     | The username of the player to get the UUID of

## MC Username from UUID 

```shell
curl "https://japi.rest/minecraft/v1/uuid/41f9049d58204631b8aa18f8397ba5c1" \
  -H "Authorization: {API KEY}"
```

```javascript
const username = '41f9049d58204631b8aa18f8397ba5c1';
const data = fetch(`https://japi.rest/minecraft/v1/uuid/${username}`, {
  headers: { "Authorization": "{API KEY}" }
}).then(res => res.json()).then(data => console.log(data));
```

> The above command returns JSON structured like this:

```json
{
  "cache_expiry": 10800,
  "cached": false,
  "data": {
    "id": "41f9049d58204631b8aa18f8397ba5c1",
    "name": "DanPlayz"
  }
}
```

This endpoint retrieves the username for a uuid from mojang.

### HTTP Request

`GET https://japi.rest/minecraft/v1/uuid/:uuid`

### Path Parameters

Parameter | Required | Description
----------|----------|----------------------------------------------
uuid      | true     | The UUID of the player to get the username of