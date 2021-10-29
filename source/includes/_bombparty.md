# BombParty

## List Information

```shell
curl "https://japi.rest/bombparty/v1/search?limit=5&sort=lenlow&q=dan" \
  -H "Authorization: {API KEY}"
```

```javascript
const word = 'dan';
const data = fetch(`https://japi.rest/bombparty/v1/search?limit=5&sort=lenlow&q=${word}`, {
  headers: { "Authorization": "{API KEY}" }
}).then(res => res.json())

console.log(data);
```

> The above command returns JSON structured like this:

```json
{
  "words": [
    "dan",
    "dang",
    "dank",
    "dans",
    "dant"
  ]
}
```

This endpoint retrieves a list of words based on the query.

### HTTP Request

`GET https://japi.rest/bombparty/v1/search`

### Query Parameters

Parameter | Required | Default | Description
----------|----------|-- |-----------------------
q         | true     | null | The word to search for
limit     | false    | 20 | The number of words to return
sort      | false    | null | The sort order of the words
lowerCase | false    | false | Whether to return the words in lowercase