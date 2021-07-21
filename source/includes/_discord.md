# Discord

## Get User

```shell
curl "https://japi.rest/discord/v1/user/:userId"
```

```javascript
const fetch = require('node-fetch'); // NodeJS users
const data = fetch("https://japi.rest/discord/v1/user/:userId").then(res => res.json())

console.log(data);
```

> The above command returns JSON structured like this:

```json
{
  "cache_expiry": 3600,
  "cached": false,
  "data": {
    "id": "209796601357533184",
    "username": "DanPlayz",
    "avatar": "49e7de8406d75a012d9add3b0383d428",
    "discriminator": "7757",
    "public_flags": 131328,
    "banner": null,
    "banner_color": "#19b9e6",
    "accent_color": 1685990,
    "avatarURL": "https://cdn.discordapp.com/avatars/209796601357533184/49e7de8406d75a012d9add3b0383d428.png",
    "bannerURL": null,
  }
}
```

This endpoint retrieves a user's information.

### HTTP Request

`GET https://japi.rest/discord/v1/user/:userId`

### Path Parameters

Parameter | Required | Description
--------- | -------- | -----------
userId    | true     | The user's ID.

## Get Template

```shell
curl "https://japi.rest/discord/v1/template/:code" \
  -H "Authorization: {API KEY}"
```

```javascript
const fetch = require('node-fetch'); // NodeJS users
const data = fetch("https://japi.rest/discord/v1/template/:code", {
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
    "code": "czqrGhSefaXQ",
    "name": "aaaaa",
    "description": "aaaa",
    "usage_count": 0,
    "creator_id": "209796601357533184",
    "creator": {
      "id": "209796601357533184",
      "username": "DanPlayz",
      "avatar": "49e7de8406d75a012d9add3b0383d428",
      "discriminator": "7757",
      "public_flags": 131328
    },
    "created_at": "2021-07-19T17:45:48+00:00",
    "updated_at": "2021-07-19T17:45:48+00:00",
    "source_guild_id": "856626398558027776",
    "serialized_source_guild": {
      "name": "Dust Test",
      "description": null,
      "region": "us-west",
      "verification_level": 0,
      "default_message_notifications": 1,
      "explicit_content_filter": 0,
      "preferred_locale": "en-US",
      "afk_timeout": 300,
      "roles": [],
      "channels": [],
      "afk_channel_id": null,
      "system_channel_id": 2,
      "system_channel_flags": 0
    },
    "is_dirty": null
  }
}
```

This endpoint retrieves a template's information.

### HTTP Request

`GET https://japi.rest/discord/v1/template/:code`

### Path Parameters

Parameter | Required | Description
--------- | -------- | -----------
code      | true     | The template code.