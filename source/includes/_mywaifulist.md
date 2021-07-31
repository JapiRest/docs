# MyWaifuList

## Waifu Information

```shell
curl "https://japi.rest/mywaifulist/v1/waifu/sylvie-4" \
  -H "Authorization: {API KEY}"
```

```javascript
const fetch = require('node-fetch'); // NodeJS users
const waifuName = 'sylvie-4';
const data = fetch(`https://japi.rest/mywaifulist/v1/waifu/${waifuName}`, {
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
    "name": "Sylvie",
    "alternateName": null,
    "gender": "female",
    "description": "Sylvie is an artist in the example Ren Py visual novel, The Question.",
    "image": "https://thicc.mywaifulist.moe/waifus/26329/ea3bf9950e1e70afc1fa0088ad3aad5cf9817b113c9e9c6081c4fc246b5aeeec_thumb.png",
    "url": "https://mywaifulist.moe/waifu/sylvie-4"
  }
}
```

This endpoint retrieves information from mywaifulist using the waifu name.

### HTTP Request

`GET https://japi.rest/mywaifulist/v1/waifu/:name`

### Path Parameters

Parameter | Required | Description
--------- | -------- | -----------
name      | true     | The waifu name

## Random Waifu Information

```shell
curl "https://japi.rest/mywaifulist/v1/random" \
  -H "Authorization: {API KEY}"
```

```javascript
const fetch = require('node-fetch'); // NodeJS users
const data = fetch(`https://japi.rest/mywaifulist/v1/random`, {
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
    "name": "Sylvie",
    "alternateName": null,
    "gender": "female",
    "description": "Sylvie is an artist in the example Ren Py visual novel, The Question.",
    "image": "https://thicc.mywaifulist.moe/waifus/26329/ea3bf9950e1e70afc1fa0088ad3aad5cf9817b113c9e9c6081c4fc246b5aeeec_thumb.png",
    "url": "https://mywaifulist.moe/waifu/sylvie-4"
  },
  "url": "https://japi.rest/mywaifulist/v1/waifu/sylvie-4"
}
```

This endpoint retrieves a article's information.

### HTTP Request

`GET https://japi.rest/mywaifulist/v1/random`

## Series Search

```shell
curl "https://japi.rest/mywaifulist/v1/series?q=village" \
  -H "Authorization: {API KEY}"
```

```javascript
const fetch = require('node-fetch'); // NodeJS users
const seriesSearch = 'village';
const data = fetch(`https://japi.rest/mywaifulist/v1/series?q=${seriesSearch}`, {
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
      "name": "The Lost Village",
      "link": "https://mywaifulist.moe/series/the-lost-village",
      "studio": null,
      "airing": {
        "start": null,
        "end": null
      },
      "waifus": 15,
      "release_date": "2016-04-01"
    },
    {
      "name": "The Zashiki Warashi of Intellectual Village",
      "link": "https://mywaifulist.moe/series/the-zashiki-warashi-of-intellectual-village",
      "studio": null,
      "airing": {
        "start": null,
        "end": null
      },
      "waifus": 1,
      "release_date": null
    },
    {
      "name": "Harvest Moon: Skytree Village",
      "link": "https://mywaifulist.moe/series/harvest-moon-skytree-village",
      "studio": null,
      "airing": {
        "start": null,
        "end": null
      },
      "waifus": 4,
      "release_date": null
    },
    {
      "name": "The Villager of Level 999 (Manga)",
      "link": "https://mywaifulist.moe/series/the-villager-of-level-999-manga",
      "studio": null,
      "airing": {
        "start": "2017-05-26",
        "end": null
      },
      "waifus": 3,
      "release_date": "2017-05-26"
    },
    {
      "name": "The Villager of Level 999 (Light Novel)",
      "link": "https://mywaifulist.moe/series/the-villager-of-level-999-light-novel",
      "studio": null,
      "airing": {
        "start": "2016-04-30",
        "end": null
      },
      "waifus": 3,
      "release_date": "2016-04-30"
    },
    {
      "name": "I Am a Villager, What About It? (Manga)",
      "link": "https://mywaifulist.moe/series/i-am-a-villager-what-about-it-manga",
      "studio": null,
      "airing": {
        "start": "2017-01-07",
        "end": null
      },
      "waifus": 3,
      "release_date": "2017-01-07"
    },
    {
      "name": "I Am a Villager, What About It?",
      "link": "https://mywaifulist.moe/series/i-am-a-villager-what-about-it",
      "studio": null,
      "airing": {
        "start": "2016-10-28",
        "end": null
      },
      "waifus": 3,
      "release_date": "2016-10-28"
    }
  ]
}
```

This endpoint retrieves the series search results from mywaifulist.

### HTTP Request

`GET https://japi.rest/mywaifulist/v1/series?q=`

### Query Parameters

Parameter | Required | Description
--------- | -------- | -----------
q         | true     | The search query

## Series Information

```shell
curl "https://japi.rest/mywaifulist/v1/series/the-lost-village" \
  -H "Authorization: {API KEY}"
```

```javascript
const fetch = require('node-fetch'); // NodeJS users
const seriesName = 'the-lost-village';
const data = fetch(`https://japi.rest/mywaifulist/v1/series/${seriesName}`, {
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
    "name": "The Lost Village",
    "description": "A bus full of eccentric individuals is headed towards the urban legend known as Nanaki Village, a place where one can supposedly start over and live a perfect life. While many have different ideas of why the village cannot be found on any map, or why even the police cannot pinpoint its location, they each look forward to their new lives and just what awaits them once they reach their destination.\n\nAfter a few mishaps, they successfully arrive at Nanaki Village only to find it completely abandoned. Judging from the state of disrepair, it has been vacant for at least a year. However, secrets are soon revealed as some of the group begin to go missing while exploring the village and amidst the confusion, they find bloody claw marks in a forest. As mistrust and in-fighting break out, will they ever be able to figure out the truth behind this lost village?",
    "image": "https://thicc.mywaifulist.moe/series/6/824380b77659815215139fac5e792adb628d3c86afd3306ee499954c2d841fd4.jpeg",
    "url": "https://mywaifulist.moe/series/the-lost-village",
    "release_date": "2016-04-01",
    "type": "TV",
    "people": [
      {
        "name": "Masaki",
        "gender": "female",
        "description": "Masaki is the main female protagonist of Mayoiga and one of the 30 individuals aboard the bus to Nan...",
        "image": "https://thicc.mywaifulist.moe/waifus/6/62853566a25b806cb21d561560bb0da240c26e595536053d5e8e809b1cfef975_thumb.jpg",
        "url": "https://mywaifulist.moe/waifu/masaki"
      },
      {
        "name": "Lovepon",
        "gender": "female",
        "description": "Not much is known about Lovepon's background except that she is trying to protect her identity. In E...",
        "image": "https://thicc.mywaifulist.moe/waifus/1754/cb56400d782ddc274088b4070b7eac93dd6d90a69f8fe4ed3d7f8b366a2d79c0_thumb.jpeg",
        "url": "https://mywaifulist.moe/waifu/lovepon"
      },
      {
        "name": "Nyanta",
        "gender": "female",
        "description": "Nyanta is one of the 30 individuals aboard the bus to Nanakimura. She is a 15-year-old student with ...",
        "image": "https://thicc.mywaifulist.moe/waifus/2129/c0a150a9f84c51cdd2ad481d200875575df15e292854f31dc8d2ab243dc0ac7b_thumb.jpeg",
        "url": "https://mywaifulist.moe/waifu/nyanta"
      },
      {
        "name": "Koharun",
        "gender": "female",
        "description": "Age: 26\r\nOccupation: graduate student\r\n\r\nShe has been researching Nanakimura for a while but couldn'...",
        "image": "https://thicc.mywaifulist.moe/waifus/3219/52d80ba776fc4577519ae8a8265bede1ef96a5f5d8a3763b029592c968306f9f_thumb.png",
        "url": "https://mywaifulist.moe/waifu/koharun"
      },
      {
        "name": "Lion",
        "gender": "female",
        "description": "Age: 14\r\n\r\nShe's usually silent and doesn't really interact much with others....",
        "image": "https://thicc.mywaifulist.moe/waifus/3223/4b839e292be6613b482cfaa0614b645835e5758196ed49b1a220e0f1f688061d_thumb.png",
        "url": "https://mywaifulist.moe/waifu/lion"
      },
      {
        "name": "Maimai",
        "gender": "female",
        "description": "Age: 17\r\nOccupation: high school student\r\n\r\nShe seems to harbor a crush on Mitsumune....",
        "image": "https://thicc.mywaifulist.moe/waifus/3225/3ed6f78ff92c17fecae00205fd78a2acad0ab87a5930da161839fbccdad61987_thumb.jpeg",
        "url": "https://mywaifulist.moe/waifu/maimai"
      },
      {
        "name": "Nanko",
        "gender": "female",
        "description": "Age: 17\r\nOccupation: detective\r\n\r\nPretty indifferent to her surroundings....",
        "image": "https://thicc.mywaifulist.moe/waifus/3227/9bd03f5cb9e61f7c1a9370a4344c48e8c241b9f3aa1619a95e0d7ab7291265ef_thumb.jpeg",
        "url": "https://mywaifulist.moe/waifu/nanko"
      },
      {
        "name": "Na-na",
        "gender": "female",
        "description": "Age: 25\r\n\r\nDreams of becoming a singer and songwriter....",
        "image": "https://thicc.mywaifulist.moe/waifus/3231/3990b92758e1d3e4420ea199afc8e4d751169b46ecbe036bb58f08f6d47c820d_thumb.png",
        "url": "https://mywaifulist.moe/waifu/na-na"
      },
      {
        "name": "Nettaiya",
        "gender": "female",
        "description": "Age: 19\r\nOccupation: Student\r\n\r\nParticipating in the tour in order to catch a break from her stalker...",
        "image": "https://thicc.mywaifulist.moe/waifus/3233/738cee3d4645e32752e24f9846b34a301a39a6679d62c84ba7fc2f7265081a82_thumb.png",
        "url": "https://mywaifulist.moe/waifu/nettaiya"
      },
      {
        "name": "Pi-tan",
        "gender": "female",
        "description": "Age: 21\r\nOccupation: Student\r\n\r\nShe and Manbe are having an affair and that is their reason for goin...",
        "image": "https://thicc.mywaifulist.moe/waifus/3235/2207bd93774734b9add0f06c009ecc40bbab0c170126c4712d83288412cafea7_thumb.png",
        "url": "https://mywaifulist.moe/waifu/pi-tan"
      },
      {
        "name": "Pu-ko",
        "gender": "female",
        "description": "Age: 16\r\nOccupation: high school student\r\n\r\nShe decided to go on a tour in search of a nice older ma...",
        "image": "https://thicc.mywaifulist.moe/waifus/3236/c0959522974c62bfd9acb72996dee8025497de21100417ed359fbd5486213032_thumb.png",
        "url": "https://mywaifulist.moe/waifu/pu-ko"
      },
      {
        "name": "Soy Latte",
        "gender": "female",
        "description": "Age: 29\r\nOccupation: Nurse\r\n\r\nShe chose to become a nurse because she wanted to help people. Under n...",
        "image": "https://thicc.mywaifulist.moe/waifus/3238/48a7616b6118febfe97f96ea09967039fde1f2bbd1693bf2ac727157690bcbc4_thumb.png",
        "url": "https://mywaifulist.moe/waifu/soy-latte"
      },
      {
        "name": "Yuune",
        "gender": "female",
        "description": "Age: 18 \r\nOccupation: high school student\r\n\r\nDoesn't have a strong personality....",
        "image": "https://thicc.mywaifulist.moe/waifus/3240/febfe39c585d3786ec7f9a18ffc44475f3b865d9e45d3a892e87e43af2474678_thumb.png",
        "url": "https://mywaifulist.moe/waifu/yuune"
      },
      {
        "name": "Yuuno",
        "gender": "female",
        "description": "Age: 19 \r\nOccupation: part-time worker\r\n\r\nHas a strong sense of justice....",
        "image": "https://thicc.mywaifulist.moe/waifus/3241/63ad0e4a90ce17f2420d8289968298fb9b2aa643b9826662068b73dd1cb96aa3_thumb.jpeg",
        "url": "https://mywaifulist.moe/waifu/yuuno"
      },
      {
        "name": "Hayato",
        "alternateName": "颯人",
        "gender": "female",
        "description": "One of the members in the expedition for Nanakimura village. He apparently has a quiet personality a...",
        "image": "https://thicc.mywaifulist.moe/waifus/7726/882d6c99ea0bd5cbc5e78c2df03c107b8aa218d602829444381155bbf94cb4fd_thumb.png",
        "url": "https://mywaifulist.moe/waifu/hayato"
      }
    ]
  }
}
```

This endpoint retrieves information from mywaifulist using the waifu name.

### HTTP Request

`GET https://japi.rest/mywaifulist/v1/waifu/:series`

### Path Parameters

Parameter | Required | Description
--------- | -------- | -----------
series    | true     | The series name