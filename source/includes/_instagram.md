# Instagram

## Get Instagram User

```shell
curl "https://japi.rest/instagram/v1/user/memes_1969"
```

```javascript
const data = fetch("https://japi.rest/instagram/v1/user/memes_1969").then(res => res.json())

console.log(data);
```

> The above command returns JSON structured like this:

```json
{
  "cache_expiry": 3600,
  "cached": false,
  "data": [
    {
      "seo_category_infos": [
        [
          "Beauty",
          "beauty"
        ],
        [
          "Dance & Performance",
          "dance_and_performance"
        ],
        [
          "Fitness",
          "fitness"
        ],
        [
          "Food & Drink",
          "food_and_drink"
        ],
        [
          "Home & Garden",
          "home_and_garden"
        ],
        [
          "Music",
          "music"
        ],
        [
          "Visual Arts",
          "visual_arts"
        ]
      ],
      "logging_page_id": "profilePage_10430362358",
      "show_suggested_profiles": false,
      "show_follow_dialog": false,
      "graphql": {
        "user": {
          "biography": "Memes = Life",
          "blocked_by_viewer": false,
          "restricted_by_viewer": null,
          "country_block": false,
          "external_url": null,
          "external_url_linkshimmed": null,
          "edge_followed_by": {
            "count": 43
          },
          "fbid": "17841410390753795",
          "followed_by_viewer": false,
          "edge_follow": {
            "count": 2
          },
          "follows_viewer": false,
          "full_name": "Just Another Meme Account",
          "has_ar_effects": false,
          "has_clips": false,
          "has_guides": false,
          "has_channel": false,
          "has_blocked_viewer": false,
          "highlight_reel_count": 0,
          "has_requested_viewer": false,
          "hide_like_and_view_counts": false,
          "id": "10430362358",
          "is_business_account": true,
          "is_professional_account": true,
          "is_joined_recently": false,
          "business_address_json": null,
          "business_contact_method": null,
          "business_email": null,
          "business_phone_number": null,
          "business_category_name": "General Interest",
          "overall_category_name": null,
          "category_enum": "MEDIA",
          "category_name": "Media",
          "is_private": false,
          "is_verified": false,
          "edge_mutual_followed_by": {
            "count": 0,
            "edges": []
          },
          "profile_pic_url": "https://scontent-lax3-1.cdninstagram.com/v/t51.2885-19/s150x150/70808195_647148179145924_7544162737492852736_n.jpg?_nc_ht=scontent-lax3-1.cdninstagram.com&_nc_ohc=ymVNGaqDfMkAX_TAh0T&edm=ABfd0MgBAAAA&ccb=7-4&oh=a222b89e84b93b78d6ec9f430c90c8c0&oe=61237A7D&_nc_sid=7bff83",
          "profile_pic_url_hd": "https://scontent-lax3-1.cdninstagram.com/v/t51.2885-19/s320x320/70808195_647148179145924_7544162737492852736_n.jpg?_nc_ht=scontent-lax3-1.cdninstagram.com&_nc_ohc=ymVNGaqDfMkAX_TAh0T&edm=ABfd0MgBAAAA&ccb=7-4&oh=9b87be93e98581bb3af0b5fc93116ce2&oe=6123CFCD&_nc_sid=7bff83",
          "requested_by_viewer": false,
          "should_show_category": true,
          "should_show_public_contacts": false,
          "username": "memes_1969",
          "connected_fb_page": null,
          "edge_felix_video_timeline": {
            "count": 0,
            "page_info": {
              "has_next_page": false,
              "end_cursor": null
            },
            "edges": []
          },
          "edge_owner_to_timeline_media": {
            "count": 120,
            "page_info": {
              "has_next_page": true,
              "end_cursor": "QVFCcl8zSjBMMTZnSFd5Y01aazhlZVFMemJJTlhic1VDd3RuVFlEeXVzV3BmYTJtNTY2MDFYU08xdkJjZEkwMkU3U3E0YTdkd1ZIVXVBNS03X3E4M0RFRA=="
            },
            "edges": [
              {
                "node": {
                  "__typename": "GraphImage",
                  "id": "2580406755878857222",
                  "shortcode": "CPPckXcLWoG",
                  "dimensions": {
                    "height": 1106,
                    "width": 1080
                  },
                  "display_url": "https://scontent-lax3-1.cdninstagram.com/v/t51.2885-15/e35/191148181_502902577573418_6450667914545997451_n.jpg?_nc_ht=scontent-lax3-1.cdninstagram.com&_nc_cat=102&_nc_ohc=C3CBgmCzq1cAX9rTMuc&edm=ABfd0MgBAAAA&ccb=7-4&oh=39fc1e10aaeb6a456534cb2b26fb4655&oe=61240320&_nc_sid=7bff83",
                  "edge_media_to_tagged_user": {
                    "edges": []
                  },
                  "fact_check_overall_rating": null,
                  "fact_check_information": null,
                  "gating_info": null,
                  "sharing_friction_info": {
                    "should_have_sharing_friction": false,
                    "bloks_app_url": null
                  },
                  "media_overlay_info": null,
                  "media_preview": "ACkq0LaygeJWZASRyef8aJLO2xhQisD3J/xqzZ/6lP8AdFSSKoBYgE/T/Dn8aVjWUnzPV7vr5matnFn5hFjr1PT257+9KtnESMiP3xu9D7/j+mathgeqr044Pbj+7Uke1uy59gfx6gUWFd9395nizixyIzx2znoenP8APmucxXatGoBIABwew9K5HbUS8jroLm5tX03+Z1Nl/qI/90VNIpYYGMd85/Qiq9kf9Hj/AN0VNIRt5G4en+fTrWhxPd+rIQMDPOfo/wDU/rUsakcjGO+d39TVdVxxjjr93vj13VPFgdsH1xgfzNAdCZ/un6H+Vcn5z+prqJWIXgZ6556DHWuO3VnI7cPZc1/L9TqbI/uI/wDdFNmjAO485/2V4/EmuYW4lUAB2AHQBjj+dOFzKTgux/4Ef8as5GtfmdIuB0AHvhPyOD3pUTPGP0X/ABrnPOkH8TfmaQ3Eo6Ow/wCBH/GgaVkdaTtQj/ZP8q4vNbGmzO/mBmZsL3JPr61i1Mjalpf5H//Z",
                  "owner": {
                    "id": "10430362358",
                    "username": "memes_1969"
                  },
                  "is_video": false,
                  "has_upcoming_event": false,
                  "accessibility_caption": "Photo by Just Another Meme Account on May 23, 2021. May be an image of text that says 'Signs and who they should date Aries: Libra Taurus: Pisces Gemini: Libra Cancer: Aquariuis Leo: Libra Virgo: Nobody Libra: Leo Scorpio: Aries Sagittarius: Capricorn Capricorn: Sagittarius Aquarius: Cancer Pisces: Taurus + 96.6K'.",
                  "edge_media_to_caption": {
                    "edges": [
                      {
                        "node": {
                          "text": "Tiktok is very interesting. Everyday something new pops up."
                        }
                      }
                    ]
                  },
                  "edge_media_to_comment": {
                    "count": 0
                  },
                  "comments_disabled": false,
                  "taken_at_timestamp": 1621828477,
                  "edge_liked_by": {
                    "count": 6
                  },
                  "edge_media_preview_like": {
                    "count": 6
                  },
                  "location": null,
                  "thumbnail_src": "https://scontent-lax3-1.cdninstagram.com/v/t51.2885-15/sh0.08/e35/c0.10.847.847a/s640x640/191148181_502902577573418_6450667914545997451_n.jpg?_nc_ht=scontent-lax3-1.cdninstagram.com&_nc_cat=102&_nc_ohc=C3CBgmCzq1cAX9rTMuc&edm=ABfd0MgBAAAA&ccb=7-4&oh=0fef7edc76b41ce61422931b60721fb9&oe=612402F0&_nc_sid=7bff83",
                  "thumbnail_resources": [
                    {
                      "src": "https://scontent-lax3-1.cdninstagram.com/v/t51.2885-15/e35/c0.10.847.847a/s150x150/191148181_502902577573418_6450667914545997451_n.jpg?_nc_ht=scontent-lax3-1.cdninstagram.com&_nc_cat=102&_nc_ohc=C3CBgmCzq1cAX9rTMuc&edm=ABfd0MgBAAAA&ccb=7-4&oh=34a91e1a1eea283daf30c9a7d1f47270&oe=6122EC5C&_nc_sid=7bff83",
                      "config_width": 150,
                      "config_height": 150
                    },
                    {
                      "src": "https://scontent-lax3-1.cdninstagram.com/v/t51.2885-15/e35/c0.10.847.847a/s240x240/191148181_502902577573418_6450667914545997451_n.jpg?_nc_ht=scontent-lax3-1.cdninstagram.com&_nc_cat=102&_nc_ohc=C3CBgmCzq1cAX9rTMuc&edm=ABfd0MgBAAAA&ccb=7-4&oh=c1f09a18d6f643d08f4cd78d31f9cc42&oe=6124549E&_nc_sid=7bff83",
                      "config_width": 240,
                      "config_height": 240
                    },
                    {
                      "src": "https://scontent-lax3-1.cdninstagram.com/v/t51.2885-15/e35/c0.10.847.847a/s320x320/191148181_502902577573418_6450667914545997451_n.jpg?_nc_ht=scontent-lax3-1.cdninstagram.com&_nc_cat=102&_nc_ohc=C3CBgmCzq1cAX9rTMuc&edm=ABfd0MgBAAAA&ccb=7-4&oh=f37ca638bce22ded3f36555a40b8cea6&oe=61243224&_nc_sid=7bff83",
                      "config_width": 320,
                      "config_height": 320
                    },
                    {
                      "src": "https://scontent-lax3-1.cdninstagram.com/v/t51.2885-15/e35/c0.10.847.847a/s480x480/191148181_502902577573418_6450667914545997451_n.jpg?_nc_ht=scontent-lax3-1.cdninstagram.com&_nc_cat=102&_nc_ohc=C3CBgmCzq1cAX9rTMuc&edm=ABfd0MgBAAAA&ccb=7-4&oh=6a957ae80704da08817d1ea08b0ef8c3&oe=61241025&_nc_sid=7bff83",
                      "config_width": 480,
                      "config_height": 480
                    },
                    {
                      "src": "https://scontent-lax3-1.cdninstagram.com/v/t51.2885-15/sh0.08/e35/c0.10.847.847a/s640x640/191148181_502902577573418_6450667914545997451_n.jpg?_nc_ht=scontent-lax3-1.cdninstagram.com&_nc_cat=102&_nc_ohc=C3CBgmCzq1cAX9rTMuc&edm=ABfd0MgBAAAA&ccb=7-4&oh=0fef7edc76b41ce61422931b60721fb9&oe=612402F0&_nc_sid=7bff83",
                      "config_width": 640,
                      "config_height": 640
                    }
                  ],
                  "coauthor_producers": []
                }
              },
              {
                "node": {
                  "__typename": "GraphImage",
                  "id": "2433128417754107119",
                  "shortcode": "CHENWeZJEzv",
                  "dimensions": {
                    "height": 631,
                    "width": 1080
                  },
                  "display_url": "https://scontent-lax3-2.cdninstagram.com/v/t51.2885-15/e35/123168166_398543181510066_1495412063261577122_n.jpg?_nc_ht=scontent-lax3-2.cdninstagram.com&_nc_cat=106&_nc_ohc=yvNvxuPnJ4EAX-w6otn&edm=ABfd0MgBAAAA&ccb=7-4&oh=55f0775cfc526afd1a71afab175edbab&oe=61228A3E&_nc_sid=7bff83",
                  "edge_media_to_tagged_user": {
                    "edges": []
                  },
                  "fact_check_overall_rating": null,
                  "fact_check_information": null,
                  "gating_info": null,
                  "sharing_friction_info": {
                    "should_have_sharing_friction": false,
                    "bloks_app_url": null
                  },
                  "media_overlay_info": null,
                  "media_preview": "ACoY2jvPIVufcf8AxdAEmfut+Y/+LqG61JICUUFnHXsBxnk/T0rGkvpiwd3K46AdPy7/AI0Abjlt6jY38X8QPb/e/wAKjNwN5jz847bhn1/v+nvUVtPJdKC3yOC6ggcj5Rzg9+fpUA0lJIzIzsWIzk8/XOetL0H6misoJ24JbrgOucfTfU/mOP4G/Nf/AIqsWzs49ySxyZIPK8HsevcccV0NCBmZd6as26RSfMbGMnjgdOnQ1Ja6fHbgMRuk7secH29PyzRRTETygl0xx97n04rGngu40IbMoz0Tpj/d6n9aKKTVyk2ndE2nW7O/nsCiqMIp47YJx6enqefrt0UULQTdz//Z",
                  "owner": {
                    "id": "10430362358",
                    "username": "memes_1969"
                  },
                  "is_video": false,
                  "has_upcoming_event": false,
                  "accessibility_caption": "Photo by Just Another Meme Account on November 01, 2020. May be a meme of text that says 'How the bed feels when I'm trying to sleep How the bed feels when I need to get up'.",
                  "edge_media_to_caption": {
                    "edges": [
                      {
                        "node": {
                          "text": "Hard to fall asleep, even harder to get outta bed"
                        }
                      }
                    ]
                  },
                  "edge_media_to_comment": {
                    "count": 0
                  },
                  "comments_disabled": false,
                  "taken_at_timestamp": 1604271531,
                  "edge_liked_by": {
                    "count": 1
                  },
                  "edge_media_preview_like": {
                    "count": 1
                  },
                  "location": null,
                  "thumbnail_src": "https://scontent-lax3-2.cdninstagram.com/v/t51.2885-15/e35/c172.0.484.484a/123168166_398543181510066_1495412063261577122_n.jpg?_nc_ht=scontent-lax3-2.cdninstagram.com&_nc_cat=106&_nc_ohc=yvNvxuPnJ4EAX-w6otn&edm=ABfd0MgBAAAA&ccb=7-4&oh=846d99dfd9bf18c0e9b1d12cc17282d2&oe=6122D8E8&_nc_sid=7bff83",
                  "thumbnail_resources": [
                    {
                      "src": "https://scontent-lax3-2.cdninstagram.com/v/t51.2885-15/e35/c172.0.484.484a/s150x150/123168166_398543181510066_1495412063261577122_n.jpg?_nc_ht=scontent-lax3-2.cdninstagram.com&_nc_cat=106&_nc_ohc=yvNvxuPnJ4EAX-w6otn&edm=ABfd0MgBAAAA&ccb=7-4&oh=e58a91d2ee3277e1735ae22005bc574e&oe=61241D0D&_nc_sid=7bff83",
                      "config_width": 150,
                      "config_height": 150
                    },
                    {
                      "src": "https://scontent-lax3-2.cdninstagram.com/v/t51.2885-15/e35/c172.0.484.484a/s240x240/123168166_398543181510066_1495412063261577122_n.jpg?_nc_ht=scontent-lax3-2.cdninstagram.com&_nc_cat=106&_nc_ohc=yvNvxuPnJ4EAX-w6otn&edm=ABfd0MgBAAAA&ccb=7-4&oh=51e74eb18b623ad487d5868784009493&oe=6123DD8B&_nc_sid=7bff83",
                      "config_width": 240,
                      "config_height": 240
                    },
                    {
                      "src": "https://scontent-lax3-2.cdninstagram.com/v/t51.2885-15/e35/c172.0.484.484a/s320x320/123168166_398543181510066_1495412063261577122_n.jpg?_nc_ht=scontent-lax3-2.cdninstagram.com&_nc_cat=106&_nc_ohc=yvNvxuPnJ4EAX-w6otn&edm=ABfd0MgBAAAA&ccb=7-4&oh=3a45b968e91f4ad4040d2c8ae89427db&oe=6122B575&_nc_sid=7bff83",
                      "config_width": 320,
                      "config_height": 320
                    },
                    {
                      "src": "https://scontent-lax3-2.cdninstagram.com/v/t51.2885-15/e35/c172.0.484.484a/s480x480/123168166_398543181510066_1495412063261577122_n.jpg?_nc_ht=scontent-lax3-2.cdninstagram.com&_nc_cat=106&_nc_ohc=yvNvxuPnJ4EAX-w6otn&edm=ABfd0MgBAAAA&ccb=7-4&oh=0051fe3c96eb5a0f126aa9eec63fb7c5&oe=6123ED74&_nc_sid=7bff83",
                      "config_width": 480,
                      "config_height": 480
                    },
                    {
                      "src": "https://scontent-lax3-2.cdninstagram.com/v/t51.2885-15/e35/c172.0.484.484a/123168166_398543181510066_1495412063261577122_n.jpg?_nc_ht=scontent-lax3-2.cdninstagram.com&_nc_cat=106&_nc_ohc=yvNvxuPnJ4EAX-w6otn&edm=ABfd0MgBAAAA&ccb=7-4&oh=846d99dfd9bf18c0e9b1d12cc17282d2&oe=6122D8E8&_nc_sid=7bff83",
                      "config_width": 640,
                      "config_height": 640
                    }
                  ],
                  "coauthor_producers": []
                }
              }
            ]
          },
          "edge_saved_media": {
            "count": 0,
            "page_info": {
              "has_next_page": false,
              "end_cursor": null
            },
            "edges": []
          },
          "edge_media_collections": {
            "count": 0,
            "page_info": {
              "has_next_page": false,
              "end_cursor": null
            },
            "edges": []
          },
          "edge_related_profiles": {
            "edges": []
          }
        }
      },
      "toast_content_on_load": null,
      "show_view_shop": false,
      "profile_pic_edit_sync_props": null,
      "always_show_message_button_to_pro_account": false
    }
  ]
}
```

This endpoint retrieves data from instagram for a given user.

### HTTP Request

`GET https://japi.rest/instagram/v1/user/:username`

### Path Parameters

Parameter  | Required   | Description
---------- | ---------- | -----------
username   | true       | The user's username.