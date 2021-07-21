# WikiHow

## Search

```shell
curl "https://japi.rest/wikihow/v1/search?q=How+to+eat+food" \
  -H "Authorization: {API KEY}"
```

```javascript
const fetch = require('node-fetch'); // NodeJS users
const search = 'How to eat food';
const data = fetch(`https://japi.rest/wikihow/v1/search/?q=${search}`, {
  headers: { "Authorization": "{API KEY}" }
}).then(res => res.json())

console.log(data);
```

> The above command returns JSON structured like this:

```json
{
  "cache_expiry": 3600,
  "cached": false,
  "data": [
    {
      "title": "How to Write Software Documentation",
      "link": "https://www.wikihow.com/Write-Software-Documentation",
      "thumbnail": "https://www.wikihow.com/images/thumb/f/fd/Write-Software-Documentation-Step-8.jpg/-crop-250-145-193px-Write-Software-Documentation-Step-8.jpg",
      "stats": {
        "views": 303499,
        "last_updated": "Updated 6 months ago"
      }
    },
    {
      "title": "How to Write a Business Process Document",
      "link": "https://www.wikihow.com/Write-a-Business-Process-Document",
      "thumbnail": "https://www.wikihow.com/images/thumb/4/4e/Apply-for-Unemployment-Compensation-in-Florida-Step-18.jpg/-crop-250-145-193px-Apply-for-Unemployment-Compensation-in-Florida-Step-18.jpg",
      "stats": {
        "views": 347086,
        "last_updated": "Updated 1 year ago"
      }
    },
    {
      "title": "How to Write a Requirements Document",
      "link": "https://www.wikihow.com/Write-a-Requirements-Document",
      "thumbnail": "https://www.wikihow.com/images/thumb/2/20/Write-a-Requirements-Document-Step-10.jpg/-crop-250-145-193px-Write-a-Requirements-Document-Step-10.jpg",
      "stats": {
        "views": 202132,
        "last_updated": "Updated 1 year ago"
      }
    }
  ]
}
```

This endpoint retrieves a user's information.

### HTTP Request

`GET https://japi.rest/wikihow/v1/search?q=`

### Query Parameters

Parameter | Required | Description
--------- | -------- | -----------
q         | true     | The search query