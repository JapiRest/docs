# Discord

## Discord User

```shell
curl "https://japi.rest/discord/v1/user/:userId"
```

```javascript
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
    "banner": "b1d92b8e931a1eaa5bd8ad6b1423851e",
    "banner_color": "#19b9e6",
    "accent_color": 1685990,
    "tag": "DanPlayz#7757",
    "createdAt": "2016-08-01T22:16:47.596Z",
    "createdTimestamp": 1470089807596,
    "public_flags_array": [
      "HOUSE_BALANCE",
      "EARLY_VERIFIED_BOT_DEVELOPER"
    ],
    "defaultAvatarURL": "https://cdn.discordapp.com/embed/avatars/2.png",
    "avatarURL": "https://cdn.discordapp.com/avatars/209796601357533184/49e7de8406d75a012d9add3b0383d428.png",
    "bannerURL": "https://cdn.discordapp.com/banners/209796601357533184/b1d92b8e931a1eaa5bd8ad6b1423851e.png"
  },
  "presence": {
    "status": "online",
    "activities": [],
    "clientStatus": [
      "desktop"
    ]
  },
  "connections": {}
}
```

This endpoint retrieves a user's information.

### HTTP Request

`GET https://japi.rest/discord/v1/user/:userId`

### Path Parameters

Parameter | Required | Description
--------- | -------- | -----------
userId    | true     | The user's ID.

## Discord User Avatar

```shell
curl "https://japi.rest/discord/v1/user/:userId/avatar"
```

```javascript
const data = fetch("https://japi.rest/discord/v1/user/:userId/avatar").then(res => res.url)

console.log(data);
```

> This endpoint is designed for web pages and uses client-side redirection.

This endpoint retrieves a user's avatar.

### HTTP Request

`GET https://japi.rest/discord/v1/user/:userId/avatar`

### Path Parameters

Parameter | Required | Description
--------- | -------- | -----------
userId    | true     | The user's ID.

### Query Parameters

Parameter | Required | Default | Description
--------- | -------- | ------- | -----------
animated  | false    | false   | Returns the avatar as gif if available.
size      | false    | 128     | Changes the size of the image, same as discord.

## Discord User Banner

```shell
curl "https://japi.rest/discord/v1/user/:userId/banner"
```

```javascript
const data = fetch("https://japi.rest/discord/v1/user/:userId/banner").then(res => res.url)

console.log(data);
```

> This endpoint is designed for web pages and uses client-side redirection.

This endpoint retrieves a user's banner.

### HTTP Request

`GET https://japi.rest/discord/v1/user/:userId/banner`

### Path Parameters

Parameter | Required | Description
--------- | -------- | -----------
userId    | true     | The user's ID.

### Query Parameters

Parameter | Required | Default | Description
--------- | -------- | ------- | -----------
animated  | false    | false   | Returns the avatar as gif if available.
size      | false    | 128     | Changes the size of the image, same as discord.


## Discord Template

```shell
curl "https://japi.rest/discord/v1/template/:code" \
  -H "Authorization: {API KEY}"
```

```javascript
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

## Discord Application

```shell
curl "https://japi.rest/discord/v1/application/:applicationId"
```

```javascript
const data = fetch("https://japi.rest/discord/v1/application/:applicationId").then(res => res.json())

console.log(data);
```

> The above command returns JSON structured like this:

```json
{
  "cache_expiry": 3600,
  "cached": false,
  "data": {
    "application": {
      "id": "587152333519978559",
      "name": "Primo",
      "icon": "747655dc3da9f544a87bb85d616e4520",
      "description": "Primo was crafted to be useable by anyone, so you never have a boring moment on discord with (or without) your friends!\n\nWebsite: https://primo.enx.so\nInvite: https://primo.enx.so/invite",
      "summary": "Primo was crafted to be useable by anyone, so you never have a boring moment on discord with (or without) your friends!\n\nWebsite: https://primo.enx.so\nInvite: https://primo.enx.so/invite",
      "type": null,
      "hook": true,
      "bot_public": true,
      "bot_require_code_grant": false,
      "terms_of_service_url": "https://primo.enx.so/terms",
      "privacy_policy_url": "https://primo.enx.so/privacy",
      "custom_install_url": "https://discord.com/oauth2/authorize?client_id=587152333519978559&permissions=2147482871&redirect_uri=http%3A%2F%2Fprimo.enx.so%2Fcallback&response_type=code&scope=bot%20identify%20guilds%20applications.commands",
      "verify_key": "9553417d309f6fce0b84a761c14b9a9a4694ba6834bb0e3533385b6ab14ba81a",
      "flags": 323584,
      "tags": [
        "fun",
        "logging",
        "moderation",
        "social",
        "utility"
      ],
      "flags_array": [
        "GATEWAY_PRESENCE",
        "GATEWAY_PRESENCE_LIMITED",
        "GATEWAY_GUILD_MEMBERS",
        "GATEWAY_GUILD_MEMBERS_LIMITED",
        "GATEWAY_MESSAGE_CONTENT"
      ],
      "assets": []
    },
    "bot": {
      "id": "587152333519978559",
      "username": "Primo",
      "avatar": "068c34bbc2357ee9c742c4c38ead9d4e",
      "discriminator": "5049",
      "public_flags": 65536,
      "bot": true,
      "approximate_guild_count": 265,
      "public_flags_array": [
        "VERIFIED_BOT"
      ]
    }
  }
}
```

This endpoint retrieves a user's information.

### HTTP Request

`GET https://japi.rest/discord/v1/application/:applicationId`

### Path Parameters

Parameter | Required | Description
--------- | -------- | -----------
applicationId    | true     | The application's ID. (A bot ID is a valid application ID)
