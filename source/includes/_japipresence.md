# JAPI Presence

## Get Presence

```shell
curl "https://japi.rest/presence/v1/get?id=209796601357533184"
```

```javascript
const fetch = require('node-fetch'); // NodeJS users
const data = fetch("https://japi.rest/presence/v1/get?id=209796601357533184").then(res => res.json())

console.log(data);
```

> The above command returns JSON structured like this:

```json
{
  "cache_expiry": 300,
  "cached": true,
  "data": {
    "sessionType": "vscode",
    "workspaceFolder": "void",
    "file": {
      "path": "/void/beta/JAPI-Docs/source/includes/_japipresence.md",
      "name": "_japipresence.md",
      "size": {
        "ctime": 1628299422775,
        "mtime": 1628300472949,
        "size": 1080,
        "type": 1
      },
      "totalLines": "47",
      "currentLine": "1",
      "currentColumn": "1"
    },
    "git": {
      "link": "https://github.com/JapiRest/docs.japi.rest/",
      "branch": "main"
    }
  }
}
```

This endpoint retrieves a user's presence who is using the [JAPI Presence](https://marketplace.visualstudio.com/items?itemName=japirest.japi-presence) Visual Studio Code Extension.

### HTTP Request

`GET https://japi.rest/presence/v1/get?id=:identifier`

### Path Parameters

Parameter  | Required | Description
---------- | -------- | -----------
identifier | true     | The user's JAPI identifier.