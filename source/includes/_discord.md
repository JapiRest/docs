# Discord

## Discord User

```shell
curl "https://japi.rest/discord/v1/user/:userId"
```

```javascript
const data = fetch("https://japi.rest/discord/v1/user/:userId").then(res => res.json()).then(data => console.log(data));
```

> The above command returns JSON structured like this:

```json
{
  "cache_expiry": 3600,
  "cached": false,
  "data": {
    "id": "209796601357533184",
    "username": "compiles",
    "avatar": "e1d1b1f8fbb78de3cb4dd6349c5b1b8a",
    "discriminator": "0",
    "public_flags": 4325632,
    "flags": 4325632,
    "banner": "f0e8349cea9efe849fca257109d96e95",
    "accent_color": 4369109,
    "global_name": "Dan",
    "avatar_decoration_data": null,
    "banner_color": "#42aad5",
    "clan": null,
    "tag": "compiles#0",
    "createdAt": "2016-08-01T22:16:47.596Z",
    "createdTimestamp": 1470089807596,
    "public_flags_array": [
      "HOUSE_BALANCE",
      "EARLY_VERIFIED_BOT_DEVELOPER",
      "ACTIVE_DEVELOPER",
      "NITRO"
    ],
    "defaultAvatarURL": "https://cdn.discordapp.com/embed/avatars/0.png",
    "avatarURL": "https://cdn.discordapp.com/avatars/209796601357533184/e1d1b1f8fbb78de3cb4dd6349c5b1b8a.png",
    "bannerURL": "https://cdn.discordapp.com/banners/209796601357533184/f0e8349cea9efe849fca257109d96e95.png"
  },
  "presence": {
    "status": "online",
    "activities": [
      {
        "name": "Custom Status",
        "type": 4,
        "url": null,
        "details": null,
        "state": "Hello!",
        "applicationId": null,
        "timestamps": null,
        "party": null,
        "syncId": null,
        "assets": null,
        "flags": 0,
        "emoji": {
          "animated": null,
          "name": "👋",
          "id": null,
          "createdTimestamp": null,
          "url": null,
          "identifier": "%F0%9F%91%8B"
        },
        "buttons": [],
        "createdTimestamp": 1721030968928
      }
    ],
    "clientStatus": [
      "desktop"
    ]
  },
  "connections": {
    "error": "Get connections via the endpoint: '/discord/v1/user/:userId/connections'"
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
}).then(res => res.json()).then(data => console.log(data));
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
const data = fetch("https://japi.rest/discord/v1/application/:applicationId").then(res => res.json()).then(data => console.log(data));
```

> The above command returns JSON structured like this:

```json
{
  "cache_expiry": 14400,
  "cached": false,
  "data": {
    "application": {
      "id": "587152333519978559",
      "name": "Primo",
      "icon": "747655dc3da9f544a87bb85d616e4520",
      "description": "Primo was crafted to be useable by anyone, so you never have a boring moment on discord with (or without) your friends!\n\nWebsite: https://primo.enx.so\nSupport: https://discord.gg/KkS6yP8",
      "summary": "",
      "type": null,
      "is_monetized": false,
      "hook": true,
      "guild_id": "658086225441456128",
      "storefront_available": false,
      "bot_public": true,
      "bot_require_code_grant": false,
      "terms_of_service_url": "https://primo.enx.so/terms",
      "privacy_policy_url": "https://primo.enx.so/privacy",
      "install_params": {
        "scopes": [
          "applications.commands",
          "bot"
        ],
        "permissions": "1642824465655"
      },
      "integration_types_config": {
        "0": {}
      },
      "verify_key": "9553417d309f6fce0b84a761c14b9a9a4694ba6834bb0e3533385b6ab14ba81a",
      "flags": 323584,
      "tags": [
        "fun",
        "logging",
        "moderation",
        "social",
        "utility"
      ],
      "assets": [],
      "flags_array": [
        "GATEWAY_PRESENCE",
        "GATEWAY_PRESENCE_LIMITED",
        "GATEWAY_GUILD_MEMBERS",
        "GATEWAY_GUILD_MEMBERS_LIMITED",
        "GATEWAY_MESSAGE_CONTENT"
      ],
      "iconURL": "https://cdn.discordapp.com/app-icons/587152333519978559/747655dc3da9f544a87bb85d616e4520.png",
      "coverURL": null,
      "createdAt": "2019-06-09T05:33:45.074Z",
      "createdTimestamp": 1560058425074,
      "installURL": "https://discord.com/api/oauth2/authorize?client_id=587152333519978559&permissions=1642824465655&scope=applications.commands%20bot"
    },
    "bot": {
      "id": "587152333519978559",
      "username": "Primo",
      "global_name": null,
      "avatar": "068c34bbc2357ee9c742c4c38ead9d4e",
      "avatar_decoration_data": null,
      "discriminator": "5049",
      "public_flags": 65536,
      "clan": null,
      "bot": true,
      "approximate_guild_count": 411,
      "createdAt": "2019-06-09T05:33:45.074Z",
      "createdTimestamp": 1560058425074,
      "public_flags_array": [
        "VERIFIED_BOT"
      ],
      "defaultAvatarURL": "https://cdn.discordapp.com/embed/avatars/4.png",
      "avatarURL": "https://cdn.discordapp.com/avatars/587152333519978559/068c34bbc2357ee9c742c4c38ead9d4e.png"
    },
    "app_discovery": {
      "id": "587152333519978559",
      "name": "Primo",
      "icon": "747655dc3da9f544a87bb85d616e4520",
      "description": "Primo was crafted to be useable by anyone, so you never have a boring moment on discord with (or without) your friends!\n\nWebsite: https://primo.enx.so\nSupport: https://discord.gg/KkS6yP8",
      "summary": "",
      "type": null,
      "is_monetized": false,
      "bot": {
        "id": "587152333519978559",
        "username": "Primo",
        "global_name": null,
        "avatar": "068c34bbc2357ee9c742c4c38ead9d4e",
        "avatar_decoration_data": null,
        "discriminator": "5049",
        "public_flags": 65536,
        "clan": null,
        "bot": true,
        "banner": "e29ebf9f6fde2fbaaed38c523873365e",
        "banner_color": null,
        "accent_color": null
      },
      "hook": true,
      "guild_id": "658086225441456128",
      "storefront_available": false,
      "bot_public": true,
      "bot_require_code_grant": false,
      "terms_of_service_url": "https://primo.enx.so/terms",
      "privacy_policy_url": "https://primo.enx.so/privacy",
      "install_params": {
        "scopes": [
          "applications.commands",
          "bot"
        ],
        "permissions": "1642824465655"
      },
      "integration_types_config": {
        "0": {}
      },
      "verify_key": "9553417d309f6fce0b84a761c14b9a9a4694ba6834bb0e3533385b6ab14ba81a",
      "flags": 323584,
      "guild": {
        "id": "658086225441456128",
        "name": "Attendant.gg",
        "icon": "241b17c8c70851e0b6567c09d5422a48",
        "description": null,
        "home_header": null,
        "splash": null,
        "discovery_splash": null,
        "features": [
          "AUTOMOD_TRIGGER_USER_PROFILE",
          "GUILD_ONBOARDING_EVER_ENABLED",
          "DEVELOPER_SUPPORT_SERVER",
          "THREADS_ENABLED",
          "PREVIEW_ENABLED",
          "GUESTS_ENABLED",
          "GUILD_ONBOARDING_HAS_PROMPTS",
          "NEWS",
          "COMMUNITY",
          "MEMBER_VERIFICATION_GATE_ENABLED",
          "AUTO_MODERATION",
          "GUILD_ONBOARDING",
          "SOUNDBOARD",
          "NEW_THREAD_PERMISSIONS",
          "CHANNEL_ICON_EMOJIS_GENERATED"
        ],
        "approximate_member_count": 301,
        "approximate_presence_count": 39
      },
      "tags": [
        "fun",
        "logging",
        "moderation",
        "social",
        "utility"
      ],
      "categories": [
        {
          "id": 8,
          "name": "Moderation and Tools"
        }
      ],
      "directory_entry": {
        "guild_count": 414,
        "detailed_description": "**Primo Bot**\n=============\n\n**About Primo**\n-----------\n\nPrimo was crafted to be use-able by anyone, whether you have knowledge of discord or not. It has a easy to use prefix and command layout. Primo's commands are fun so you'll never have a boring moment on discord with your friends!\n\n**Features**\n-----------\n\n• Moderation Commands  \n• Reaction Commands  \n• Wordscan Command Scan users custom status for words.  \n• Chat Games  \n• Social Media Commands\n• Translate command  \n• Dashboard\n• All commands can be disabled/enabled!\n\n  \n  \n\n[Invite](http://primo.enx.so/invite) • [Commands](http://primo.enx.so/commands) • [Dashboard](http://primo.enx.so/dashboard)",
        "detailed_description_localizations": null,
        "supported_locales": [
          "en-US"
        ],
        "external_urls": [
          {
            "name": "Website",
            "url": "https://primo.enx.so"
          },
          {
            "name": "Commands",
            "url": "https://primo.enx.so/commands"
          },
          {
            "name": "Dashboard",
            "url": "https://primo.enx.so/dashboard"
          }
        ],
        "short_description": "Primo is a multi-purpose bot that was created to be useable by anyone, whether you have knowledge of discord or not.",
        "short_description_localizations": null
      }
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
