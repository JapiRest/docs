# Wordle

## Get Current Wordle

```shell
curl "https://japi.rest/wordle/v1/get" \
  -H "Authorization: {API KEY}"
```

```javascript
const data = fetch(`https://japi.rest/wordle/v1/get`, {
  headers: { "Authorization": "{API KEY}" }
}).then(res => res.json()).then(data => console.log(data));
```

> The above command returns JSON structured like this:

```json
{
  "cache_expiry": 300,
  "cached": false,
  "data": {
    "yesterday": {
      "date": "2022-04-27",
      "number": 312,
      "word": "heist"
    },
    "today": {
      "date": "2022-04-28",
      "number": 313,
      "word": "shown"
    },
    "tomorrow": {
      "date": "2022-04-29",
      "number": 314,
      "word": "zesty"
    }
  }
}
```

This endpoint retrieves the search results from wikihow.

### HTTP Request

`GET https://japi.rest/wordle/v1/get`
