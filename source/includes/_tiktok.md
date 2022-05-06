# TikTok

## Tiktok Creator

```shell
curl "https://japi.rest/tiktok/v1/creator/@dumcrap" \
  -H "Authorization: {API KEY}"
```

```javascript
const creator = 'dumcrap';
const data = fetch(`https://japi.rest/tiktok/v1/creator/@${creator}`, {
  headers: { "Authorization": "{API KEY}" }
}).then(res => res.json()).then(data => console.log(data));
```

> The above command returns JSON structured like this:

```json
{
  "cache_expiry":3600,
  "cached":false,
  "data":{
     "meta":{
        "title":"Poof 😘 (@dumcrap) TikTok | Watch Poof 😘's Newest TikTok Videos",
        "keywords":"Poof 😘,dumcrap,TikTok, ティックトック, tik tok, tick tock, tic tok, tic toc, tictok, тик ток, ticktock",
        "description":"Poof 😘 (@dumcrap) on TikTok | 3.3K Likes. 89 Fans. Want a cookie? 🍪 Watch the latest video from Poof 😘 (@dumcrap).",
        "canonicalHref":"https://www.tiktok.com/@dumcrap",
        "robotsContent":"index, follow",
        "applicableDevice":"pc, mobile"
     },
     "user":{
        "user":{
           "id":"6790129596711224326",
           "shortId":"0",
           "uniqueId":"dumcrap",
           "nickname":"Poof 😘",
           "avatarLarger":"https://p16-sign-va.tiktokcdn.com/musically-maliva-obj/1665263781858309~c5_1080x1080.jpeg?x-expires=1630965600&x-signature=0ZA%2Br%2BcT1nY6IqBS4Okrp%2FmVnE0%3D",
           "avatarMedium":"https://p16-sign-va.tiktokcdn.com/musically-maliva-obj/1665263781858309~c5_720x720.jpeg?x-expires=1630965600&x-signature=NI6M8vHoWxlv2W%2Fidlz7AMxftnI%3D",
           "avatarThumb":"https://p16-sign-va.tiktokcdn.com/musically-maliva-obj/1665263781858309~c5_100x100.jpeg?x-expires=1630965600&x-signature=ojckG%2BH0U%2Fe7OIwY4bO9uDRd%2FPw%3D",
           "signature":"Want a cookie? 🍪",
           "createTime":1580950461,
           "verified":false,
           "secUid":"MS4wLjABAAAA-jRfqGFJPc-4NmoS6H_X4g_XKCT80Ebo5FG5A4MlU-USR8dPy0Jgb11uubT8hulH",
           "ftc":false,
           "relation":0,
           "openFavorite":false,
           "commentSetting":0,
           "duetSetting":0,
           "stitchSetting":0,
           "privateAccount":false,
           "secret":false,
           "isADVirtual":false,
           "roomId":""
        },
        "stats":{
           "followerCount":89,
           "followingCount":6,
           "heart":3276,
           "heartCount":3276,
           "videoCount":35,
           "diggCount":0
        },
        "itemList":[
           
        ]
     },
     "videos":[
        {
           "id":"6956711554943323397",
           "desc":"Yikes #fyp #ludwig #livestreamclips #clips #clip #inappropriate #funny #meme #dankmeme",
           "createTime":1619735633,
           "scheduleTime":0,
           "video":{
              "id":"6956711554943323397",
              "height":1024,
              "width":576,
              "duration":50,
              "ratio":"720p",
              "cover":"https://p16-sign-va.tiktokcdn.com/obj/tos-maliva-p-0068/c2f3943d51d9492e9b24343183164b28?x-expires=1630900800&x-signature=K71VOjegT3xSPudgu9U2qY4u1Jk%3D",
              "originCover":"https://p16-sign-va.tiktokcdn.com/obj/tos-maliva-p-0068/cfb6c7c93c21433c8877d84b52caf70b_1619735635?x-expires=1630900800&x-signature=FzFWSKiYbt5ZHTLxCZ6pFlQ9FAk%3D",
              "dynamicCover":"https://p16-sign-va.tiktokcdn.com/obj/tos-maliva-p-0068/046d0771e7734c18b61eac7273435fb4_1619735635?x-expires=1630900800&x-signature=aVEoUxYt9LSmr0VWlYim5GbhA7M%3D",
              "playAddr":"https://v16-web.tiktok.com/video/tos/useast2a/tos-useast2a-ve-0068c001/73b4a9873f7b42209e9c640690788302/?a=1988&br=838&bt=419&cd=0%7C0%7C0&ch=0&cr=0&cs=0&dr=0&ds=3&er=&expire=1630903398&ft=9wMeReta4kag3&l=2021090522422801018803222332AF84BE&lr=tiktok_m&mime_type=video_mp4&net=0&pl=0&policy=3&qs=0&rc=ank0bTVsZjptNTMzNzczM0ApNTplNDUzMzwzN2U7OGdkNWdpcWtnYV41NTJgLS1kMTZzczYvMV9jLTIyYy1gLV8uYl86Yw%3D%3D&signature=9b1bcde07e6018ecb1c89c293b66e4d3&tk=0&vl=&vr=",
              "downloadAddr":"https://v16-web.tiktok.com/video/tos/useast2a/tos-useast2a-ve-0068c001/73b4a9873f7b42209e9c640690788302/?a=1988&br=838&bt=419&cd=0%7C0%7C0&ch=0&cr=0&cs=0&dr=0&ds=3&er=&expire=1630903398&ft=9wMeReta4kag3&l=2021090522422801018803222332AF84BE&lr=tiktok_m&mime_type=video_mp4&net=0&pl=0&policy=3&qs=0&rc=ank0bTVsZjptNTMzNzczM0ApNTplNDUzMzwzN2U7OGdkNWdpcWtnYV41NTJgLS1kMTZzczYvMV9jLTIyYy1gLV8uYl86Yw%3D%3D&signature=9b1bcde07e6018ecb1c89c293b66e4d3&tk=0&vl=&vr=",
              "shareCover":[
                 "",
                 "https://p16-sign-va.tiktokcdn.com/tos-maliva-p-0068/cfb6c7c93c21433c8877d84b52caf70b_1619735635~tplv-tiktok-play.jpeg?x-expires=1630900800&x-signature=RPi8UejfcWcGSsBEmSerj%2BVi6nI%3D",
                 "https://p16-sign-va.tiktokcdn.com/tos-maliva-p-0068/cfb6c7c93c21433c8877d84b52caf70b_1619735635~tplv-tiktokx-share-play.jpeg?x-expires=1630900800&x-signature=HTxAkwhwBSHllimV2CqgoJURQKc%3D"
              ],
              "reflowCover":"https://p16-sign-va.tiktokcdn.com/obj/tos-maliva-p-0068/c2f3943d51d9492e9b24343183164b28?x-expires=1630900800&x-signature=K71VOjegT3xSPudgu9U2qY4u1Jk%3D",
              "bitrate":429869,
              "encodedType":"normal",
              "format":"mp4",
              "videoQuality":"normal",
              "encodeUserTag":"",
              "codecType":"h264",
              "definition":"720p"
           },
           "author":{
              "id":"6790129596711224326",
              "shortId":"0",
              "uniqueId":"dumcrap",
              "nickname":"Poof 😘",
              "avatarLarger":"https://p16-sign-va.tiktokcdn.com/musically-maliva-obj/1665263781858309~c5_1080x1080.jpeg?x-expires=1630965600&x-signature=0ZA%2Br%2BcT1nY6IqBS4Okrp%2FmVnE0%3D",
              "avatarMedium":"https://p16-sign-va.tiktokcdn.com/musically-maliva-obj/1665263781858309~c5_720x720.jpeg?x-expires=1630965600&x-signature=NI6M8vHoWxlv2W%2Fidlz7AMxftnI%3D",
              "avatarThumb":"https://p16-sign-va.tiktokcdn.com/musically-maliva-obj/1665263781858309~c5_100x100.jpeg?x-expires=1630965600&x-signature=ojckG%2BH0U%2Fe7OIwY4bO9uDRd%2FPw%3D",
              "signature":"Want a cookie? 🍪",
              "createTime":1580950461,
              "verified":false,
              "secUid":"MS4wLjABAAAA-jRfqGFJPc-4NmoS6H_X4g_XKCT80Ebo5FG5A4MlU-USR8dPy0Jgb11uubT8hulH",
              "ftc":false,
              "relation":0,
              "openFavorite":false,
              "commentSetting":0,
              "duetSetting":0,
              "stitchSetting":0,
              "privateAccount":false,
              "secret":false,
              "isADVirtual":false,
              "roomId":""
           },
           "music":{
              "id":"6956711419358317318",
              "title":"original sound",
              "playUrl":"https://sf16-ies-music-va.tiktokcdn.com/obj/musically-maliva-obj/6956711521288325893.mp3",
              "coverLarge":"https://p16-sign-va.tiktokcdn.com/musically-maliva-obj/1665263781858309~c5_1080x1080.jpeg?x-expires=1630965600&x-signature=0ZA%2Br%2BcT1nY6IqBS4Okrp%2FmVnE0%3D",
              "coverMedium":"https://p16-sign-va.tiktokcdn.com/musically-maliva-obj/1665263781858309~c5_720x720.jpeg?x-expires=1630965600&x-signature=NI6M8vHoWxlv2W%2Fidlz7AMxftnI%3D",
              "coverThumb":"https://p16-sign-va.tiktokcdn.com/musically-maliva-obj/1665263781858309~c5_100x100.jpeg?x-expires=1630965600&x-signature=ojckG%2BH0U%2Fe7OIwY4bO9uDRd%2FPw%3D",
              "authorName":"Poof 😘",
              "original":true,
              "duration":50,
              "album":"",
              "scheduleSearchTime":0
           },
           "challenges":[
              {
                 "id":"229207",
                 "title":"fyp",
                 "desc":"",
                 "profileLarger":"",
                 "profileMedium":"",
                 "profileThumb":"",
                 "coverLarger":"",
                 "coverMedium":"",
                 "coverThumb":"",
                 "isCommerce":false
              },
           ],
           "stats":{
              "diggCount":72,
              "shareCount":3,
              "commentCount":2,
              "playCount":969
           },
           "duetInfo":{
              "duetFromId":"0"
           },
           "warnInfo":[
              
           ],
           "originalItem":false,
           "officalItem":false,
           "textExtra":[
              {
                 "awemeId":"",
                 "start":6,
                 "end":10,
                 "hashtagId":"229207",
                 "hashtagName":"fyp",
                 "type":1,
                 "userId":"",
                 "isCommerce":false,
                 "userUniqueId":"",
                 "secUid":""
              },
           ],
           "secret":false,
           "forFriend":false,
           "digged":false,
           "itemCommentStatus":0,
           "showNotPass":false,
           "vl1":false,
           "takeDown":0,
           "itemMute":false,
           "effectStickers":[
              
           ],
           "authorStats":{
              "followerCount":89,
              "followingCount":6,
              "heart":3276,
              "heartCount":3276,
              "videoCount":35,
              "diggCount":1427
           },
           "privateItem":false,
           "duetEnabled":true,
           "stitchEnabled":true,
           "stickersOnItem":[
              
           ],
           "isAd":false,
           "shareEnabled":true,
           "comments":[
              
           ],
           "duetDisplay":0,
           "stitchDisplay":0
        },
     ]
  }
}
```

This endpoint retrieves a tiktok creator's profile data.

### HTTP Request

`GET https://japi.rest/tiktok/v1/creator/:creator`

### Path Parameters

Parameter | Required | Description
--------- | -------- | -----------
creator   | true     | The creator username with @
