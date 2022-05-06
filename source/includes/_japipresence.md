# JAPI Presence

## Get Presence

```shell
curl "https://japi.rest/presence/v1/get?id=209796601357533184"
```

```javascript
const data = fetch("https://japi.rest/presence/v1/get?id=209796601357533184").then(res => res.json()).then(data => console.log(data));
```

> The above command returns JSON structured like this:

```json
{
  "cache_expiry": 300,
  "cached": true,
  "data": {
    "presenceVersion": "0.3.0",
    "sessionType": "vscode",
    "workspaceFolder": "void",
    "dirName": "includes",
    "file": {
      "path": "/void/beta/JAPI-Docs/source/includes/_japipresence.md",
      "name": "_japipresence.md",
      "extension": ".md",
      "extensionImage": "https://github.com/vscode-icons/vscode-icons/blob/master/icons/file_type_md.svg",
      "size": "1.33kb",
      "totalLines": "54",
      "currentLine": "20",
      "currentColumn": "17"
    },
    "git": {
      "repoName": "",
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