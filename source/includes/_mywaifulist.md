# MyWaifuList

## Waifu Information

```shell
curl "https://japi.rest/mywaifulist/v1/waifu/sylvie-4" \
  -H "Authorization: {API KEY}"
```

```javascript
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
    "id": 26329,
    "slug": "sylvie-4",
    "name": "Sylvie",
    "original_name": "",
    "romaji_name": "",
    "display_picture": "https://thicc.mywaifulist.moe/waifus/26329/ea3bf9950e1e70afc1fa0088ad3aad5cf9817b113c9e9c6081c4fc246b5aeeec_thumb.png",
    "description": "Sylvie is an artist in the example Ren Py visual novel, The Question.",
    "weight": null,
    "height": null,
    "bust": null,
    "hip": null,
    "waist": null,
    "blood_type": null,
    "origin": null,
    "age": 0,
    "birthday_month": "",
    "birthday_day": 0,
    "birthday_year": "",
    "likes": 1,
    "trash": 1,
    "popularity_rank": 29187,
    "like_rank": 30514,
    "trash_rank": 21800,
    "husbando": false,
    "nsfw": false,
    "creator": {
      "id": 52140,
      "name": "WaifuAdder420"
    },
    "tags": [],
    "url": "https://www.mywaifulist.moe/waifu/sylvie-4",
    "appearances": [
      {
        "name": "Ren'Py",
        "original_name": null,
        "romaji_name": "",
        "description": "A visual novel engine",
        "slug": "ren-py",
        "airing_start": null,
        "airing_end": null,
        "episode_count": null,
        "release": null,
        "display_picture": "https://thicc.mywaifulist.moe/series/4563/c60ae44bcb66c927051ccbf278ebe92bae73b71b4a454eb7d27f8f576736fd29.jpeg",
        "studio": null
      }
    ],
    "series": {
      "name": "Ren'Py",
      "original_name": null,
      "romaji_name": "",
      "description": "A visual novel engine",
      "slug": "ren-py",
      "airing_start": null,
      "airing_end": null,
      "episode_count": null,
      "release": null,
      "display_picture": "https://thicc.mywaifulist.moe/series/4563/c60ae44bcb66c927051ccbf278ebe92bae73b71b4a454eb7d27f8f576736fd29.jpeg",
      "studio": null
    }
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
curl "https://japi.rest/mywaifulist/v1/waifu/random" \
  -H "Authorization: {API KEY}"
```

```javascript
const data = fetch(`https://japi.rest/mywaifulist/v1/waifu/random`, {
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
    "id": 26329,
    "slug": "sylvie-4",
    "name": "Sylvie",
    "original_name": "",
    "romaji_name": "",
    "display_picture": "https://thicc.mywaifulist.moe/waifus/26329/ea3bf9950e1e70afc1fa0088ad3aad5cf9817b113c9e9c6081c4fc246b5aeeec_thumb.png",
    "description": "Sylvie is an artist in the example Ren Py visual novel, The Question.",
    "weight": null,
    "height": null,
    "bust": null,
    "hip": null,
    "waist": null,
    "blood_type": null,
    "origin": null,
    "age": 0,
    "birthday_month": "",
    "birthday_day": 0,
    "birthday_year": "",
    "likes": 1,
    "trash": 1,
    "popularity_rank": 29187,
    "like_rank": 30514,
    "trash_rank": 21800,
    "husbando": false,
    "nsfw": false,
    "creator": {
      "id": 52140,
      "name": "WaifuAdder420"
    },
    "tags": [],
    "url": "https://www.mywaifulist.moe/waifu/sylvie-4",
    "appearances": [
      {
        "name": "Ren'Py",
        "original_name": null,
        "romaji_name": "",
        "description": "A visual novel engine",
        "slug": "ren-py",
        "airing_start": null,
        "airing_end": null,
        "episode_count": null,
        "release": null,
        "display_picture": "https://thicc.mywaifulist.moe/series/4563/c60ae44bcb66c927051ccbf278ebe92bae73b71b4a454eb7d27f8f576736fd29.jpeg",
        "studio": null
      }
    ],
    "series": {
      "name": "Ren'Py",
      "original_name": null,
      "romaji_name": "",
      "description": "A visual novel engine",
      "slug": "ren-py",
      "airing_start": null,
      "airing_end": null,
      "episode_count": null,
      "release": null,
      "display_picture": "https://thicc.mywaifulist.moe/series/4563/c60ae44bcb66c927051ccbf278ebe92bae73b71b4a454eb7d27f8f576736fd29.jpeg",
      "studio": null
    }
  }
}
```

This endpoint retrieves a article's information.

### HTTP Request

`GET https://japi.rest/mywaifulist/v1/waifu/random`

## Series Search

```shell
curl "https://japi.rest/mywaifulist/v1/series?q=village" \
  -H "Authorization: {API KEY}"
```

```javascript
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

## Top Tier Waifus

```shell
curl "https://japi.rest/mywaifulist/v1/best" \
  -H "Authorization: {API KEY}"
```

```javascript
const data = fetch(`https://japi.rest/mywaifulist/v1/best`, {
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
      "name": "Eleonora Viltaria",
      "id": 2483,
      "slug": "eleonora-viltaria-lord-marksman-and-vanadis-madan-no-ou-to-vanadis",
      "description": "Previously a mercenary, Eleonora is a war maiden of the Leitmeritz. She leads the Silver Meteor army with her sword that controls the wind. She made Tigre the \"main protagonist\" fight under her, and in her own funny way she develops feelings for him, or maybe it was for his bow skills.\r\n\r\nShe owns a dragon.\r\n\r\nEleonora Viltaria, who also known as Elen, is the main female protagonist of Madan no Ou no Vanadis series and one of seven Vanadis in the story. Renowned for her valor and honor, Elen vows to protect Zhcted from any enemy threats as her life depends on it. She is also one of Tigre's prominent ally after she captured him as a \"prisoner of war\", who later readily to fight for her name, thus creating a bond between the Alsace's Earl the Wind Vanadis. Being one of main commanders of the Silver Meteor Army and the Moonlight Knights, Elen is also a former member of the Silver Gale Mercenaries and an adopted daughter of its late leader Vissarion.",
      "likes": 204,
      "trash": 7,
      "display_picture": "https://thicc.mywaifulist.moe/waifus/2483/10d0cabe6babbbb469301e8fddd42cbf2ebebd70de81d4a7fe4a72004c1756b0_thumb.jpeg",
      "appearances": [
        {
          "slug": "lord-marksman-and-vanadis",
          "name": "Lord Marksman and Vanadis",
          "root_name": "Lord Marksman and Vanadis"
        }
      ],
      "popularity_rank": 2343,
      "like_rank": 2002,
      "trash_rank": 9271,
      "weighted_ratio": 0.9331
    },
    {
      "name": "Ai Hayasaka",
      "id": 5106,
      "slug": "ai-hayasaka-kaguya-sama-love-is-war",
      "description": "Ai Hayasaka is one of the protagonists in the Kaguya-sama wa Kokurasetai series. She is a third-year student at Shuchi'in Academy and a former employee of the Shinomiya Group who served as Kaguya Shinomiya's valet.\n\nAi is a beautiful, young girl with blonde hair that is usually tied up at the left side of her head with a blue scrunchie and blue-eyes. She alters her appearance and choice of clothing to suit different roles and carry out her duties as Kaguya's valet. She wears a maid outfit when tending to the Shinomiya household. As a student at Shuchi'in Academy, she wears a modified high school uniform to match up with kogal fashion and a sweater wrapped around her waist. As Haysaca-chan, she dresses up in a Firis Girls' High sailor uniform with her hair down and a small braid tied on the right side, while as Haysaca-kun, she sports a butler uniform and a short, black hair wig. During the class trip, she cut off her ponytail to prevent one of Un'yo Shinomiya's men from continuing to hold on to it. She ends up styling it into a bob with a star and crescent moon hairpin on the left side, her old scrunchie now being used as a wristband on her left hand.\n\nDespite her young age, Ai can quickly shift to different types of personalities to suit various kinds of situations and scenarios. She has four distinct personas which, aside from having a specific purpose, has its own unique background and upbringing. As a maid, she is level-headed who carries out duties flawlessly and while she occasionally give her mistress grief over her absurd demands, she still loves her deeply. In her school camouflage version, she is a fashion-conscious schoolgirl with a penchant for rule-breaking and her liveliness is her trademark. The anti-Miyuki version, Haysaca-chan, is a doe-eyed maneater who picks up men in Roponggi and Azabu and leads them around by the nose. Haysaca-kun exists to counter the unpredictable Chika Fujiwara and has the backstory of an Irish orphan who later graduated at Harvard then ended up as a butler who becomes a crybaby when remembering his past. In reality, she is just a kind girl who deeply loves her mistress, whom she considers a sister and is willing to go against the Shinomiya house within reason like sneaking Kaguya out of the main house to see the summer fireworks. She is also known to be very sensitive about the fact that she never had any experience of dating a guy. Since the Kyoto class trip, Hayasaka seems to have dropped her gyaru persona around her friends, who now see her as somewhat distant and harsh. They interpret this as a sign of heartbreak.",
      "likes": 3956,
      "trash": 244,
      "display_picture": "https://thicc.mywaifulist.moe/waifus/5106/6df0aed1adbee07ab563456af45da5a72592c48c4717a8e7c8bf1bfd63e8a8d6_thumb.jpeg",
      "appearances": [
        {
          "slug": "kaguya-sama-love-is-war",
          "name": "Kaguya-sama: Love is War",
          "root_name": "Kaguya-sama: Love is War"
        },
        {
          "slug": "kaguya-sama-love-is-war-season-2",
          "name": "Kaguya-sama: Love is War Season 2",
          "root_name": "Kaguya-sama: Love is War"
        }
      ],
      "popularity_rank": 22,
      "like_rank": 20,
      "trash_rank": 205,
      "weighted_ratio": 0.9344
    },
    {
      "name": "Satan",
      "id": 7079,
      "slug": "satan",
      "description": "Satan is the Demon King of Wrath, known for terrible anger.\r\nLady Satan is always engaged in an eternal battle against the angel legions, and likes war more than her three meals.\r\nWith a personality that gets anxious over the little details, she’s dangerous because she’s always irritated. However, it might be wise not to be hard on her. She has a weakness for cute animals, and is another one that doesn’t have a clear head.",
      "likes": 125,
      "trash": 3,
      "display_picture": "https://thicc.mywaifulist.moe/waifus/7079/393334272fdf01f72e53851074989a81b0520a8eca29d19b2bb2f8233be1afb4_thumb.png",
      "appearances": [
        {
          "slug": "seven-mortal-sins",
          "name": "Seven Mortal Sins",
          "root_name": "Seven Mortal Sins"
        }
      ],
      "popularity_rank": 3861,
      "like_rank": 3258,
      "trash_rank": 14589,
      "weighted_ratio": 0.9334
    },
    {
      "name": "Moriko Morioka",
      "id": 7913,
      "slug": "moriko-morioka",
      "description": "\r\nShe has quit the company she's been working on since high school and turned into a 30-year-old single NEET. She spends her days in a net game in search for the satisfaction that otherwise she can't obtain in real life.",
      "likes": 312,
      "trash": 13,
      "display_picture": "https://thicc.mywaifulist.moe/waifus/7913/eab5741396dfab08bbe8d6b6ca41d20f7b40b33e7cc7a2eaf533d447bdc358b8_thumb.jpg",
      "appearances": [
        {
          "slug": "net-juu-no-susume",
          "name": "Net-juu no Susume",
          "root_name": "Net-juu no Susume"
        }
      ],
      "popularity_rank": 1460,
      "like_rank": 1229,
      "trash_rank": 5966,
      "weighted_ratio": 0.9328
    },
  ]
}
```

This endpoint retrieves the "Top Tier Waifus" from mywaifulist.

### HTTP Request

`GET https://japi.rest/mywaifulist/v1/best`

## Most Popular

```shell
curl "https://japi.rest/mywaifulist/v1/popular" \
  -H "Authorization: {API KEY}"
```

```javascript
const data = fetch(`https://japi.rest/mywaifulist/v1/popular`, {
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
      "name": "Megumin",
      "id": 319,
      "slug": "megumin-konosuba-god-s-blessing-on-this-wonderful-world",
      "description": "Megumin is an Arch Wizard of the Crimson Demon Clan in the Fantasy World and is the first person to join Kazuma's party. She is one of the main characters of the KonoSuba series.\n\nMegumin is a young girl with shoulder-length dark brown hair (smooth black in light novel) and crimson colored eyes. She wears a classical witch attire such as a black cloak with gold border, choker, wizard's hat, fingerless gloves, and carries a black staff. Though she jokingly claims that her eyepatch seals her immense power, she sees it as a stylish sense of fashion due to her chuunibyou tendencies.\n\nShe has a fair skin and a light complexion. Unlike her rival Yunyun who has a more developed body, Megumin seems to have a delicate under-developed figure, as Kazuma describes her figure as a \"porcelain doll\". Yuiyui also stated that all of their family members have a thin body, but Megumin thinks that it's just because they lack nutrients because they hardly eat solid food.\n\nMegumin is a straightforward girl, who speaks in an old-style Japanese dialect. She can be very hyper and lively at times and has chuunibyou tendencies like the rest of the Crimson Demon villagers. She is very intelligent, but has very little self-control, especially when it comes to using Explosion magic. She has no problem wasting her spell on empty plains or abandoned castles, as long as she can use Explosion once a day.\n\nShe decided to become an Explosion mage after a busty older woman saved her with Explosion magic when she was young, and after learning it claims she \"must cast Explosion once a day or die.\"\n\nWhile still attending school, Megumin would swindle food from Yunyun everyday since her parents couldn't afford meals. Due to her exceptional academic performance, Megumin was able to graduate early. When she left to travel alone, Yunyun predicted she would be \"at a loss due to a lack in the means of survival, begging a useless guy for a meal.\"\n\nAfter traveling to Axel Town, she quickly gained a reputation as a crazy Explosion fanatic, thus parties refused to accept her before meeting Kazuma and Aqua.",
      "likes": 11429,
      "trash": 2357,
      "display_picture": "https://thicc.mywaifulist.moe/waifus/319/812a2f1f3592b967987637e373229112b2ff89cd38f34c2feaae119c1e63c0f1_thumb.jpeg",
      "appearances": [
        {
          "slug": "konosuba-god-s-blessing-on-this-wonderful-world",
          "name": "KonoSuba: God’s Blessing on this Wonderful World!",
          "root_name": "KonoSuba: God’s Blessing on this Wonderful World!"
        }
      ],
      "popularity_rank": 1,
      "like_rank": 1,
      "trash_rank": 6,
      "weighted_ratio": null
    },
    {
      "name": "Rem",
      "id": 41,
      "slug": "rem-re-zero-starting-life-in-another-world",
      "description": "Rem is a maid in service of lord Roswaal L Mathers, alongside her sister, Ram. She is one of the main supporting characters of Re:Zero, with major roles in Arc 2, Arc 3, and Arc 7. During the first half of Arc 2, she also served as the secondary antagonist. While initially distrustful of Subaru, she eventually opened up to him and even developed strong feelings for him after he saved her. However, at the end of Arc 3, she had her name and memories eaten by Lye Batenkaitos and subsequently fell into suspended animation. At the end of Arc 6, she finally woke up from her slumber following Lye's death, but now suffers amnesia due to not having regained her memories yet. She has been transported to the Empire of Vollacia with Subaru and Louis Arneb at the start of Arc 7.\n\nRem has medium length sky blue hair that covers her right eye, large light blue eyes, and young features. She also has hair clips towards the left side of her hair, a flower-shaped ribbon on the same side of her hair, and a maid hairband. She looks nearly identical to her sister apart from her hair, eyes, and ribbon colouring. She usually wears a maid uniform, and since her chest is slightly larger than her sister's, she secretly changes the measurements to hide it.\n\nRem tends to speak in a superficially polite manner and sometimes acts without thinking. She holds both, respect to the point of worship and guilt toward her sister for an incident in the past. Because of her respect and guilt toward her sister, she used to think of herself as inferior. After Subaru saves her, she falls deeply in love with him, becoming one of his most loyal followers. Rem will stick with him no matter what happens, even if Subaru rejects himself. After having awoken from an almost two year long slumber, Rem's memories were completely erased, leaving her in a state similar to that of Crusch at the end of Arc 3. She's very wary of everyone, especially Subaru, even going as far as trying to strangle him twice and set up decoy paths and traps in order to get away from him, as she considers him dangerous due to a combination of the overwhelming Witch's Miasma seaping from him after his numerous deaths, as well as his resentment for the last Archbishop of Gluttony and refusal to help her in her current state, for Rem sees Louis as just an innocent child.",
      "likes": 9203,
      "trash": 2316,
      "display_picture": "https://thicc.mywaifulist.moe/waifus/41/0202153e3a8b44ee5833dfc5b4c1f9dc9b3791a13d61787ed28d6a72319f4138_thumb.png",
      "appearances": [
        {
          "slug": "re-zero-starting-life-in-another-world",
          "name": "Re:ZERO -Starting Life in Another World-",
          "root_name": "Re:ZERO -Starting Life in Another World-"
        },
        {
          "slug": "re-zero-starting-life-in-another-world-season-2",
          "name": "Re:ZERO -Starting Life in Another World- Season 2",
          "root_name": "Re:ZERO -Starting Life in Another World-"
        },
        {
          "slug": "re-zero-starting-life-in-another-world-season-2-part-2",
          "name": "Re:ZERO -Starting Life in Another World- Season 2 Part 2",
          "root_name": "Re:ZERO -Starting Life in Another World-"
        }
      ],
      "popularity_rank": 2,
      "like_rank": 2,
      "trash_rank": 7,
      "weighted_ratio": null
    },
  ]
}
```

This endpoint retrieves the "Most Popular" from mywaifulist.

### HTTP Request

`GET https://japi.rest/mywaifulist/v1/popular`

## Top Trash

```shell
curl "https://japi.rest/mywaifulist/v1/trash" \
  -H "Authorization: {API KEY}"
```

```javascript
const data = fetch(`https://japi.rest/mywaifulist/v1/trash`, {
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
      "name": "Malty Melromarc",
      "id": 2090,
      "slug": "malty-melromarc-the-rising-of-the-shield-hero",
      "description": "Malty Melromarc, now known as Bitch, is the former first Princess of Melromarc and primary antagonist of the series.\r\n\r\nShe was first described by Naofumi as a lovely girl with semi-long crimson hair, emerald-green eyes, pretty cute and youthful facial features, yet slightly shorter than Naofumi. Even after her betrayal, Naofumi admits that she is a waste of beauty and describes her as needlessly attractive.\r\n\r\nUnder her mask, she is a narcissist egocentric, haughty, dishonest, corrupt, arrogant, amoral, treacherous, sinister, deceitful, selfish, greedy, and a compulsive liar - putting it shortly, she is basically a sociopath. She is shown to be highly adept at lying and manipulating people, and is not above insulting and making them as miserable as possible. She is deceptive enough to \"cry\" crocodile tears in order to fool people into taking her side.\r\n\r\nTo fix her bad personality, the Queen sent her to study abroad in a school at Faubley. But all that accomplished was Malty's \"graduation\" from virginity.",
      "likes": 230,
      "trash": 3616,
      "display_picture": "https://thicc.mywaifulist.moe/waifus/2090/e94dd823bf4895d1f788739261ef40bdf62e0b6ec6c1ac35a66a8eb5c5175926_thumb.jpeg",
      "appearances": [
        {
          "slug": "the-rising-of-the-shield-hero",
          "name": "The Rising of the Shield Hero",
          "root_name": "The Rising of the Shield Hero"
        }
      ],
      "popularity_rank": 24,
      "like_rank": 1773,
      "trash_rank": 2,
      "weighted_ratio": 0.9323
    },
    {
      "name": "Akemi Hinazuki",
      "id": 3907,
      "slug": "akemi-hinazuki",
      "description": "Akemi was raised by her single mother. When Kayo was still young, Akemi's husband would physically abuse her. Because of this, her mother forced her to divorce him. After that, she raised Kayo as a single parent and often took out her frustrations on her. After her abusive nature was revealed, Kayo was taken to live with her grandmother and her parental rights were taken away.",
      "likes": 61,
      "trash": 2556,
      "display_picture": "https://thicc.mywaifulist.moe/waifus/3907/b6a3d87181ef185a390b96e5fe541513a5b6d86e5d3a8e257743f8d623c3f6c7_thumb.jpeg",
      "appearances": [
        {
          "slug": "erased",
          "name": "ERASED",
          "root_name": "ERASED"
        }
      ],
      "popularity_rank": 48,
      "like_rank": 6157,
      "trash_rank": 3,
      "weighted_ratio": 0.9702
    },
  ]
}
```

This endpoint retrieves the "Top Trash" from mywaifulist.

### HTTP Request

`GET https://japi.rest/mywaifulist/v1/trash`

## Most Popular Virtual Youtubers

```shell
curl "https://japi.rest/mywaifulist/v1/vtubers" \
  -H "Authorization: {API KEY}"
```

```javascript
const data = fetch(`https://japi.rest/mywaifulist/v1/vtubers`, {
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
      "name": "Kizuna Ai",
      "id": 1608,
      "slug": "kizuna-ai-youtube",
      "description": "Kizuna Ai is the world's first virtual Youtuber. The channel name is \"A.I. Channel\" and her nickname is \"Ai-chan\". She was born on June 30 and has the same birthday as Sailor Moon and ChibiUsa.\r\n\r\nShe wears a pink headband that looks like a heart because Ai can mean \"love\". Since she is technically a newborn, she tried to look like a sprout. The front flap of her uniform has the letter \"A\" on it from \"AI\". The clothes were designed to be futuristic.\r\n\r\nBecause the clothes are actually data, they are technically covering 0% of her skin. Does this mean she is practically naked?",
      "likes": 1227,
      "trash": 139,
      "display_picture": "https://thicc.mywaifulist.moe/waifus/1608/105790f902e38da70c7ac59da446586c86eb19c7a9afc063b974d74b8870c4cc_thumb.png",
      "appearances": [
        {
          "slug": "youtube",
          "name": "YouTube",
          "root_name": "YouTube"
        },
        {
          "slug": "azur-lane-game",
          "name": "Azur Lane (Game)",
          "root_name": "Azur Lane"
        }
      ],
      "popularity_rank": 203,
      "like_rank": 177,
      "trash_rank": 460,
      "weighted_ratio": null
    },
    {
      "name": "Gura Gawr",
      "id": 32382,
      "slug": "gura-gawr-hololive-production",
      "description": "Gura Gawr is an English Virtual YouTuber associated with hololive, as part of its English (EN) branch first generation of VTubers alongside Ninomae Ina'nis, Takanashi Kiara, Watson Amelia, and Mori Calliope.\n\nGura is friendly and readily likeable, and often amuses with foolish antics. She has difficulty telling left from right; once sent the entire hololive EN digging for 20 minutes in the wrong direction because she misread a map; often misspells and mispronounces words; once mistook bread for a potato; has trouble remembering her own age; once calculated that 9+10 equals 11; and didn't recognize the term \"simp\", which she corrected to \"shrimp\".\n\nProfile:\nGura is a descendant of the Lost City of Atlantis, who swam to Earth while saying \"It's so boring down there LOLOLOL!\" She bought her clothes (and her shark hat) in the human world and she really loves them. In her spare time, she enjoys talking to marine life. Gura is over nine thousand years old, however she has forgotten her exact age some time after reaching five thousand. When asked, she will produce a random number in the nine thousands.\n\nIllust. Amashiro Natsuki\nModel: Shin Umiushi\nChannel: https://www.youtube.com/channel/UCoSrY_IQQVpmIRZ9Xf-y93g",
      "likes": 684,
      "trash": 55,
      "display_picture": "https://thicc.mywaifulist.moe/waifus/32382/a7cdc2ed940aa85e55654ec6aed62893ab3d224c0d1da6d3d8cfc57d5cf4a44f_thumb.jpeg",
      "appearances": [
        {
          "slug": "hololive-english",
          "name": "Hololive English",
          "root_name": "Hololive Production"
        }
      ],
      "popularity_rank": 519,
      "like_rank": 453,
      "trash_rank": 1650,
      "weighted_ratio": null
    },
  ]
}
```

This endpoint retrieves the "Most Popular Virtual Youtubers" from mywaifulist.

### HTTP Request

`GET https://japi.rest/mywaifulist/v1/vtubers`

## Seasonal Best Waifus

```shell
curl "https://japi.rest/mywaifulist/v1/current/best" \
  -H "Authorization: {API KEY}"
```

```javascript
const data = fetch(`https://japi.rest/mywaifulist/v1/current/best`, {
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
      "name": "Milim Nava",
      "id": 7728,
      "slug": "milim-nava-that-time-i-got-reincarnated-as-a-slime",
      "description": "Milim Nava is one of the oldest and strongest Demon Lords, and the third True Demon Lord to come into existence. She is the one and only existing Dragonoid with the nickname of \"Destroyer,\" and is often called a tyrant because of her childishly irritable personality combined with her power.\n\nEven among a dissolved group of the Ten Great Demon Lords, she is a Demon Lord one should never fight against, being the only other being, aside from Rimuru, to have the ability to use an infinite amount of Magicules.\n\nAlthough Milim is a Dragonoid, she looks like a regular human child about the age of 10 to 13, making many people confuse her a harmless existence at first.\n\nShe has glossy pink hair (white/silver in the Web Novel akin to her mother) tied in twin-tails. She usually wears a black skimpy gothic dress that barely covers her body.\n\nAfterward, she also started to wear the Dragon Knuckles that Rimuru gifted her.\n\nIn her Battle Form, Milim actually looks more like the Dragonoid that she is, having a crimson horn adorning her forehead and jet black armor adorning her body. She also sprouts wings, revealing her existence as the special, one-and-only, being that she is.\n\nShe is the most short-tempered and simple Demon Lord, what the rest would consider common sense is completely lost on her. However, though she might be a short-tempered simpleton, she is by no means stupid.\n\nThere's a possibility that she doesn't have many friends. It can be speculated that she's been living for so long that she must have lost many good friends by now.\n\nShe has a complete lack of dishonesty and is honest to an extreme. Milim probably hasn't even heard the word “negotiation”. She boldly declares her demands and rampages if they are rejected. She, unfortunately, believes that if you are working, there is no need to hide anything.\n\nMilim is the daughter of the human mother, Lucia and the Creator of the World, \"Star King Dragon\" Veldanava. Her existence is the main reason for why it is a deemed a taboo for the True Dragons to have children, because, after her birth, she inherited most of the powers from her father, making him incredibly weak. As the daughter of God, she is able to generate and use an infinite amount of Magicules due to the Magicule Breeder Reactor and is also able to use the Stardust, which is the densest form of energy in existence.",
      "likes": 1100,
      "trash": 88,
      "display_picture": "https://thicc.mywaifulist.moe/waifus/21495/788959e5be43dcea863ea095e7380b18e330f98d98ea21ae799b68a02c4972a7_thumb.jpeg",
      "appearances": [
        {
          "slug": "that-time-i-got-reincarnated-as-a-slime",
          "name": "That Time I Got Reincarnated as a Slime",
          "root_name": "That Time I Got Reincarnated as a Slime"
        },
        {
          "slug": "that-time-i-got-reincarnated-as-a-slime-ova",
          "name": "That Time I Got Reincarnated as a Slime OVA",
          "root_name": "That Time I Got Reincarnated as a Slime"
        },
        {
          "slug": "that-time-i-got-reincarnated-as-a-slime-season-2",
          "name": "That Time I Got Reincarnated as a Slime Season 2",
          "root_name": "That Time I Got Reincarnated as a Slime"
        },
        {
          "slug": "that-time-i-got-reincarnated-as-a-slime-season-2-part-ii",
          "name": "That Time I Got Reincarnated as a Slime Season 2: Part II",
          "root_name": "That Time I Got Reincarnated as a Slime"
        },
        {
          "slug": "the-slime-diaries-that-time-i-got-reincarnated-as-a-slime",
          "name": "The Slime Diaries: That Time I Got Reincarnated as a Slime",
          "root_name": "That Time I Got Reincarnated as a Slime"
        }
      ],
      "popularity_rank": 261,
      "like_rank": 217,
      "trash_rank": 874,
      "weighted_ratio": 0.9096
    },
    {
      "name": "Shuna",
      "id": 7729,
      "slug": "shuna-that-time-i-got-reincarnated-as-a-slime",
      "description": "Shuna is one of the third group of subordinate Monsters to be named by Rimuru, evolving her from an Ogre to a Kijin. She was originally the princess of the Ogre tribe and even though she had the talent for using Magic, she was a sheltered girl, but quickly got along with the Goblinas. Shuna lives in the Capital city of the Jura Tempest Federation: Rimuru City. The daughter of the late ogre chieftain and Benimaru's younger sister, which is why she's nicknamed \"Oni Princess\" by Rimuru. Very skilled and knowledgeable in domestic matters, she essentially becomes Rimuru's chief economic advisor together with Rigurd.\n\nIn her Ogre stage, Shuna was a petite girl with the appearance of a 13-14-year-old Human girl with the exception of her two large porcelain horns protruding from her forehead. She has long, wavy, pink hair, coupled with large hot-pink eyes under very light, barely existing eyebrows. She wore a simple pink kimono, covered by a similarly simple white robe that covered her arms in excess. She also had a thin, low-ponytail that was tied using a single small white ribbon. Her fair skin has a slightly pink tint alongside a couple of tear-like face markings similar to Benimaru, supposedly, to go along with her pink color scheme, with the addition of two fangs that are long enough to slightly protrude out her lips to add to the \"ferocious\" theme of the Ogres. After evolution, she took on the appearance akin to a 16-year-old human girl with a height of 155 centimeters, looking more refined and beautiful compared to her former cute self. Her horns also became narrower as with all Ogre to Kijin evolutions. The slight pink tint on her skin is gone, as well as the face markings, and fangs that are small to be only visible when she speaks. Excelling at weaving, she made herself a new white kimono with simple but graceful red embroidery and red kimono skirt that's held in place with a red ribbon.\n\nShuna is a gentle and forgiving girl with keen senses. Being raised as a princess she also has a refined and graceful personality. Rimiru tends to rely on her regal disposition when it comes to diplomacy with the leaders of other nations. She is at that age where she is happy to be depended on, hence since she was always sheltered as a little girl in the Ogre tribe, she's incredibly happy and content with her current position under Rimuru. Even a bit of responsibility seems to make her happy. Even so, she is not to be underestimated as she can get incredibly competitive in certain areas too, such as, being appointed as Rimuru's close aide and taking care of him personally. The will to do so is so much that Shuna and Shion unknowingly pull on Rimuru to the point of tearing him in half. Just like Shion, she uses every chance to cuddle with Rimuru's blob form. Shuna shows off her femininity by showing her skill in weaving silk on a loom. Shuna is made responsible for clothing everyone in their fledgling village and had already woven several rolls of silk.",
      "likes": 1072,
      "trash": 77,
      "display_picture": "https://thicc.mywaifulist.moe/waifus/7729/97dd0343ab2446c7e6c4dcb4ebebc05fe1a6574189ed1cac9ab615e7d4791421_thumb.jpg",
      "appearances": [
        {
          "slug": "that-time-i-got-reincarnated-as-a-slime",
          "name": "That Time I Got Reincarnated as a Slime",
          "root_name": "That Time I Got Reincarnated as a Slime"
        },
        {
          "slug": "that-time-i-got-reincarnated-as-a-slime-ova",
          "name": "That Time I Got Reincarnated as a Slime OVA",
          "root_name": "That Time I Got Reincarnated as a Slime"
        },
        {
          "slug": "that-time-i-got-reincarnated-as-a-slime-season-2",
          "name": "That Time I Got Reincarnated as a Slime Season 2",
          "root_name": "That Time I Got Reincarnated as a Slime"
        },
        {
          "slug": "that-time-i-got-reincarnated-as-a-slime-season-2-part-ii",
          "name": "That Time I Got Reincarnated as a Slime Season 2: Part II",
          "root_name": "That Time I Got Reincarnated as a Slime"
        },
        {
          "slug": "the-slime-diaries-that-time-i-got-reincarnated-as-a-slime",
          "name": "The Slime Diaries: That Time I Got Reincarnated as a Slime",
          "root_name": "That Time I Got Reincarnated as a Slime"
        }
      ],
      "popularity_rank": 281,
      "like_rank": 233,
      "trash_rank": 1011,
      "weighted_ratio": 0.917
    },
  ]
}
```

This endpoint retrieves the "Seasonal Best Waifus" from mywaifulist.

### HTTP Request

`GET https://japi.rest/mywaifulist/v1/current/best`

## Seasonal Worst Waifus

```shell
curl "https://japi.rest/mywaifulist/v1/current/trash" \
  -H "Authorization: {API KEY}"
```

```javascript
const data = fetch(`https://japi.rest/mywaifulist/v1/current/trash`, {
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
      "name": "Satoko Houjou",
      "id": 727,
      "slug": "satoko-houjou",
      "description": "Satoko is a younger classmate in Keiichi's school. She has a distinctive style of speech, ending all of her sentences with 'wa' which, at times, is grammatically incorrect. In spite of her young age, she is quite clever in setting up traps, and likes to practice on Keiichi. ",
      "likes": 161,
      "trash": 124,
      "display_picture": "https://thicc.mywaifulist.moe/waifus/727/85cadf378203ac2daf69cfcbfda26b69c2e576834d3d4524acaa6ebf472721e1_thumb.jpeg",
      "appearances": [
        {
          "slug": "when-they-cry",
          "name": "When They Cry",
          "root_name": "When They Cry"
        },
        {
          "slug": "when-they-cry-2020",
          "name": "When They Cry (2020)",
          "root_name": "When They Cry"
        },
        {
          "slug": "when-they-cry-sotsu",
          "name": "When They Cry - Sotsu",
          "root_name": "When They Cry"
        }
      ],
      "popularity_rank": 1690,
      "like_rank": 2531,
      "trash_rank": 531,
      "weighted_ratio": 0.3788
    },
    {
      "name": "Shouta",
      "id": 4258,
      "slug": "shouta-miss-kobayashi-s-dragon-maid",
      "description": "A boy being chased by an oppai dragon.",
      "likes": 165,
      "trash": 211,
      "display_picture": "https://thicc.mywaifulist.moe/waifus/4258/a10197750c29e1646c8cfc1df0b044a986b3b6bdd95ca9c3e159570ea426504c_thumb.jpeg",
      "appearances": [
        {
          "slug": "miss-kobayashi-s-dragon-maid",
          "name": "Miss Kobayashi's Dragon Maid",
          "root_name": "Miss Kobayashi's Dragon Maid"
        },
        {
          "slug": "miss-kobayashi-s-dragon-maid-s",
          "name": "Miss Kobayashi's Dragon Maid S",
          "root_name": "Miss Kobayashi's Dragon Maid"
        }
      ],
      "popularity_rank": 1254,
      "like_rank": 2514,
      "trash_rank": 245,
      "weighted_ratio": 0.5106
    },
    {
      "name": "Riko Saikawa",
      "id": 4259,
      "slug": "riko-saikawa",
      "description": "Riko Saikawa is one of the supporting characters in Kobayashi-san Chi no Maid Dragon and one of the main protagonist of Kobayashi-san Chi no Maid Dragon: Kanna no Nichijou. She is Kanna Kamui's friend and classmate. \n\nRiko has wavy shoulder-length brown hair. She has dark green eyes and usually dons a light-green, long sleeved shirt with a rounded yellow neckline fronted by a bunny motif, a pale orange skirt, white high socks, and green shoes. She sports a yellow-rimmed tag clipped to her shirt and an orange daisy pin in her hair. Riko appears to have an especially shiny forehead, as it gleams with a flash of light in many scenes of the anime. Much like some other characters, her outfit is prone to change in accordance with her environment, situation, and surroundings. \n\nAt first glance, Riko seems bossy and mean, but over time she seems nicer as shown with Kanna and very polite around people like Kobayashi. She has a crush on Kanna and enjoys being around her. When being touched by Kanna or receives praise from her, Riko tends to grin goofily and get red in the face, becoming overwhelmed with excitement.",
      "likes": 292,
      "trash": 261,
      "display_picture": "https://thicc.mywaifulist.moe/waifus/4259/0ccef9e9cc493d850fc34b1323292151cf78248c33f352c51e5b2a2e568b6c99_thumb.png",
      "appearances": [
        {
          "slug": "miss-kobayashi-s-dragon-maid",
          "name": "Miss Kobayashi's Dragon Maid",
          "root_name": "Miss Kobayashi's Dragon Maid"
        },
        {
          "slug": "miss-kobayashi-s-dragon-maid-s",
          "name": "Miss Kobayashi's Dragon Maid S",
          "root_name": "Miss Kobayashi's Dragon Maid"
        }
      ],
      "popularity_rank": 774,
      "like_rank": 1364,
      "trash_rank": 180,
      "weighted_ratio": 0.4307
    },
  ]
}
```

This endpoint retrieves the "Seasonal Worst Waifus" from mywaifulist.

### HTTP Request

`GET https://japi.rest/mywaifulist/v1/current/trash`

## Seasonal Most Popular Waifus

```shell
curl "https://japi.rest/mywaifulist/v1/current/popular" \
  -H "Authorization: {API KEY}"
```

```javascript
const data = fetch(`https://japi.rest/mywaifulist/v1/current/popular`, {
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
      "name": "Tohru",
      "id": 555,
      "slug": "tohru-miss-kobayashi-s-dragon-maid",
      "description": "Tohru is a female dragon with the ability to transform into a human girl. After Kobayashi rescues her, she falls in love with her and decides to work for her as a maid. She is the daughter of the Emperor of Demise.\n\nIn her human form, Tohru has long blonde hair with flaming orange tips with pink/purple added to the hair and red-orange eyes with dilated pupils, and a buxom figure with large thighs and plump, bouncy breasts, claiming to be a D cup (for dragon size). She magically transforms her scales into a maid outfit, copying the uniform from a maid cosplay cafe (Maid Cafe Cozy) after flying to Kobayashi's apartment the first time. While in the private comfort of Kobayashi's apartment, Tohru wears her tail out, and on occasion, her wings. Outside, she hides both her tail and wings but retains her horns. Anyone who notices usually chalks it up to a form of cosplay. Tohru's dragon form appears as a big green European dragon with black wings and a light green underbelly. The height of her dragon form towers over Kobayashi's old apartment that's four stories high.\n\nAs a Chaos Dragon, Tohru was raised to hate humans and is supposed to be a fierce and dangerous dragon with nothing other than destruction in mind, but this all changed when she met Kobayashi. She is now cheerful and kind to every human she meets, except for those who are a real or, as it is in most cases, imagined rival love interest to Kobayashi. She is also quickly influenced by what she sees on the television or internet. Tohru is sexually attracted to Kobayashi, telling the latter herself, and often performs acts out of sexual desire for her, such as licking her clothes clean, offering to lotion her body, and attempting multiple times to get Kobayashi to specifically eat her tail meat, despite Kobayashi claiming to be ethically against consuming.",
      "likes": 6041,
      "trash": 1079,
      "display_picture": "https://thicc.mywaifulist.moe/waifus/555/5f6e4d4e7043368da7e2235e2e300be456953cc17aabc2a9f829b9c438f374cb_thumb.jpeg",
      "appearances": [
        {
          "slug": "miss-kobayashi-s-dragon-maid",
          "name": "Miss Kobayashi's Dragon Maid",
          "root_name": "Miss Kobayashi's Dragon Maid"
        },
        {
          "slug": "miss-kobayashi-s-dragon-maid-s",
          "name": "Miss Kobayashi's Dragon Maid S",
          "root_name": "Miss Kobayashi's Dragon Maid"
        }
      ],
      "popularity_rank": 9,
      "like_rank": 8,
      "trash_rank": 27,
      "weighted_ratio": null
    },
    {
      "name": "Kanna Kamui",
      "id": 497,
      "slug": "kanna-kamui-miss-kobayashi-s-dragon-maid",
      "description": "Tohru's friend from the dragon realm who got exiled from her world and winds up living with Kobayashi as well. She is very young by dragon standards, equivalent to a elementary school girl. She initially assumes that Kobayashi seduced Tohru into staying and wanted her to return to their original world. She later grows attached to Kobayashi, viewing her as a mother figure.",
      "likes": 4453,
      "trash": 1057,
      "display_picture": "https://thicc.mywaifulist.moe/waifus/497/4e90e6c674e38512135ea995d0006e45856f1fc6cfe781fd440807ad95a33b94_thumb.jpg",
      "appearances": [
        {
          "slug": "miss-kobayashi-s-dragon-maid",
          "name": "Miss Kobayashi's Dragon Maid",
          "root_name": "Miss Kobayashi's Dragon Maid"
        },
        {
          "slug": "miss-kobayashi-s-dragon-maid-s",
          "name": "Miss Kobayashi's Dragon Maid S",
          "root_name": "Miss Kobayashi's Dragon Maid"
        }
      ],
      "popularity_rank": 17,
      "like_rank": 19,
      "trash_rank": 30,
      "weighted_ratio": null
    },
    {
      "name": "Lucoa",
      "id": 849,
      "slug": "lucoa-miss-kobayashi-s-dragon-maid",
      "description": "Also referred to as Lucoa. A dragon goddess and another friend of Tohru, lost her divine status centuries ago after getting drunk and causing a scandal, much like the Quetzalcoatl of the original myth. Appears in her human form as a tall woman with gigantic breasts.",
      "likes": 1930,
      "trash": 441,
      "display_picture": "https://thicc.mywaifulist.moe/waifus/849/c9e5a585c78be7fb1f6f04e86cdddff4f42d3082dd1aa2bb1c0685da0214b024_thumb.png",
      "appearances": [
        {
          "slug": "miss-kobayashi-s-dragon-maid",
          "name": "Miss Kobayashi's Dragon Maid",
          "root_name": "Miss Kobayashi's Dragon Maid"
        },
        {
          "slug": "miss-kobayashi-s-dragon-maid-s",
          "name": "Miss Kobayashi's Dragon Maid S",
          "root_name": "Miss Kobayashi's Dragon Maid"
        }
      ],
      "popularity_rank": 65,
      "like_rank": 71,
      "trash_rank": 79,
      "weighted_ratio": null
    },
  ]
}
```

This endpoint retrieves the "Seasonal Best Waifus" from mywaifulist.

### HTTP Request

`GET https://japi.rest/mywaifulist/v1/current/popular`