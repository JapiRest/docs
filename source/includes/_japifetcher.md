# JAPI Fetcher

<aside class="info">
  These endpoints are fetched via JAPI Fetcher.
  
  Invite it at https://bot.japi.rest/invite
  Get Support at https://bot.japi.rest/support
</aside>

## Discord User Presence

```shell
curl "https://japi.rest/discord/v1/user/:userId/presence"
```

```javascript
const data = fetch("https://japi.rest/discord/v1/user/:userId/presence").then(res => res.json())

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

## Discord Guild

```shell
curl "https://japi.rest/discord/v1/guild/733135938347073576" \
  -H "Authorization: {API KEY}"
```

```javascript
const data = fetch("https://japi.rest/discord/v1/guild/733135938347073576", {
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
    "id": "733135938347073576",
    "name": "Void Bots",
    "icon": "a_aa6362876672e26c01edbe2cfb3f0dd5",
    "features": [
      "COMMUNITY",
      "VANITY_URL",
    ],
    "commands": [],
    "members": [
      "209796601357533184",
    ],
    "channels": [
      "733135938741600361",
    ],
    "bans": [],
    "roles": [
      "733135938351398956",
    ],
    "stageInstances": [],
    "invites": [],
    "deleted": false,
    "shardId": 0,
    "splash": "a9aa17893e693998c39b3c9f5c79d249",
    "banner": "b0217bdf6bb7dd2cebb47ffb59b13ea8",
    "description": "Void Bots. Here you can find the perfect bot for your server, or add your bot!",
    "verificationLevel": "HIGH",
    "vanityURLCode": "voidbots",
    "nsfwLevel": "DEFAULT",
    "discoverySplash": "bf283eb880fd266fb74eb164b066cbcd",
    "memberCount": 2029,
    "large": true,
    "applicationId": null,
    "afkTimeout": 900,
    "afkChannelId": null,
    "systemChannelId": "749432519681900576",
    "premiumTier": "TIER_3",
    "premiumSubscriptionCount": 14,
    "explicitContentFilter": "ALL_MEMBERS",
    "mfaLevel": "ELEVATED",
    "joinedTimestamp": 1633366124703,
    "defaultMessageNotifications": "ONLY_MENTIONS",
    "systemChannelFlags": 5,
    "maximumMembers": 250000,
    "maximumPresences": null,
    "approximateMemberCount": null,
    "approximatePresenceCount": null,
    "vanityURLUses": null,
    "rulesChannelId": "761339128343167057",
    "publicUpdatesChannelId": "733135939127345227",
    "preferredLocale": "en-US",
    "ownerId": "726243005438099577",
    "emojis": [
      "733147957188362310",
    ],
    "stickers": [
      "859875867144224818",
    ],
    "createdTimestamp": 1594863628709,
    "nameAcronym": "VB",
    "iconURL": "https://cdn.discordapp.com/icons/733135938347073576/a_aa6362876672e26c01edbe2cfb3f0dd5.webp",
    "splashURL": "https://cdn.discordapp.com/splashes/733135938347073576/a9aa17893e693998c39b3c9f5c79d249.webp",
    "discoverySplashURL": "https://cdn.discordapp.com/discovery-splashes/733135938347073576/bf283eb880fd266fb74eb164b066cbcd.webp",
    "bannerURL": "https://cdn.discordapp.com/banners/733135938347073576/b0217bdf6bb7dd2cebb47ffb59b13ea8.webp"
  }
}
```

This endpoint retrieves a guild's information.

### HTTP Request

`GET https://japi.rest/discord/v1/guild/:guildid`

### Path Parameters

Parameter | Required | Description
----------|----------|--------------
guildid   | true     | The guild id.

## Discord Guild Member

```shell
curl "https://japi.rest/discord/v1/guild/733135938347073576/members/209796601357533184" \
  -H "Authorization: {API KEY}"
```

```javascript
const data = fetch("https://japi.rest/discord/v1/guild/733135938347073576/members/209796601357533184", {
  headers: { "Authorization": "{API KEY}" }
}).then(res => res.json())

console.log(data);
```

> The above command returns JSON structured like this:

```json
{
  "cache_expiry": 300,
  "cached": false,
  "data": {
    "guildId": "733135938347073576",
    "joinedTimestamp": 1594863628713,
    "premiumSinceTimestamp": 1627077775719,
    "deleted": false,
    "nickname": null,
    "pending": false,
    "userId": "209796601357533184",
    "displayName": "DanPlayz",
    "roles": [
      {
        "id": "743980331274600459",
        "name": "👑",
        "color": "#000000",
        "hoist": false,
        "rawPosition": 86,
        "managed": false,
        "mentionable": false,
        "deleted": false,
        "tags": null,
        "createdTimestamp": 1597449133462
      },
      {
        "id": "735302323835764767",
        "name": "Nitro Booster",
        "color": "#ff73fa",
        "hoist": true,
        "rawPosition": 58,
        "managed": true,
        "mentionable": false,
        "deleted": false,
        "createdTimestamp": 1595380135259
      },
      {
        "id": "733884613578981376",
        "name": "Member",
        "color": "#b9bbbe",
        "hoist": false,
        "rawPosition": 40,
        "managed": false,
        "mentionable": false,
        "deleted": false,
        "tags": null,
        "createdTimestamp": 1595042126794
      },
      {
        "id": "733135938347073576",
        "name": "@everyone",
        "color": "#000000",
        "hoist": false,
        "rawPosition": 0,
        "managed": false,
        "mentionable": false,
        "deleted": false,
        "tags": null,
        "createdTimestamp": 1594863628709
      }
    ]
  }
}
```

This endpoint retrieves a guild member's information.

### HTTP Request

`GET https://japi.rest/discord/v1/guild/:guildid/members/:memberid`

### Path Parameters

Parameter | Required | Description
----------|----------|---------------
guildid   | true     | The guild id.
memberid  | true     | The member id.