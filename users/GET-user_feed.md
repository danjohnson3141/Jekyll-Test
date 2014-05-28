<!-- --- title: GET /user_feed -->

This route is a collection of post and notifications that is specific to the active user. This list is procedurally generated based off of a variety of criteria. 


Feed is composed of:

* Posts in groups that the active user is a member of
* Posts in events that the active user is following
* Visible posts that are commented on by connected user
* Visible posts that are liked by connected user
* Visible posts that are created by connected user
* Notifciation if connected user changes their title
* Notification if connected user changes their organization
* Notification if connected user registers for visible and/or followed event
* Notification if connected user creates a visible group
* Posts the user is following

These items are sorted by the most recently created at the top of the list and then descending. Several actions that can be taken by other users can affect the order of the posts by bumping that post to the top of the list. Whether or not the user is following a post and also whether the action was taken by a connection or non-connection will affect this. If the user **is not** following the post, the action must be taken by a connection for it to affect the sort order. If the user **is** following the post, then the action does not need to be performed by a connection for the sort order to be affected.

* Comment on a visible post
* Like on a visible post
* Adding an attachment

=
####Authentication:

The user needs to be logged in and have valid credentials to use this route.

=
####Parameters:

None; default only.

=
####API request example:
```html
http://stage-api-access.evant.com/user_feed
```

=
####JSON response example:

```json
{
    "user_feed": [
        {
            "post": {
                "id": 132,
                "title": null,
                "excerpt": null,
                "generated_excerpt": "...",
                "thumbnail_teaser_photo": null,
                "view_count": 1,
                "show_likes_count": true,
                "like_count": 0,
                "comment_count": 0,
                "post_like_id": null,
                "can_like": true,
                "featured": false,
                "show_post_likes_list": true,
                "ago": "1h",
                "created_by": 7,
                "group": {
                    "id": 1,
                    "name": "CIO",
                    "group_type_name": "Open"
                },
                "event": null,
                "sponsor": null,
                "event_session": null,
                "recent_activity": null,
                "authors": [
                    {
                        "id": 7,
                        "first_name": "Graham",
                        "last_name": "Baas",
                        "title": "Quality Assurance",
                        "organization_name": "Evanta",
                        "photo": "https://s3.amazonaws.com/access_resources/staging/thumbnails/7.jpg?12",
                        "moderator": false,
                        "user_profile": true
                    }
                ],
                "post_attachments": [
                    {
                        "id": 76,
                        "post_id": 132,
                        "url": "https://s3.amazonaws.com/access_resources/staging/post_attachments/.2cf1394ce099a0e40dd8a2bede5c166f_7.pdf",
                        "created_by": 7,
                        "ago": "1h"
                    }
                ]
            },
            "notification": null
        },
        {
            "post": {
                "id": 115,
                "title": "something to add an attachment to",
                "excerpt": null,
                "generated_excerpt": "blah blah blah",
                "thumbnail_teaser_photo": null,
                "view_count": 30,
                "show_likes_count": true,
                "like_count": 2,
                "comment_count": 1,
                "post_like_id": 105,
                "can_like": true,
                "featured": false,
                "show_post_likes_list": true,
                "ago": "7d",
                "created_by": 5,
                "group": {
                    "id": 1,
                    "name": "CIO",
                    "group_type_name": "Open"
                },
                "event": null,
                "sponsor": null,
                "event_session": null,
                "recent_activity": null,
                "authors": [
                    {
                        "id": 5,
                        "first_name": "Nathan",
                        "last_name": "Brakken",
                        "title": "Web Developer",
                        "organization_name": "Evanta",
                        "photo": "https://evanta.com/Resources/contacts/large/104450.jpg",
                        "moderator": false,
                        "user_profile": true
                    }
                ],
                "post_attachments": [
                    {
                        "id": 28,
                        "post_id": 115,
                        "url": "https://s3.amazonaws.com/access_resources/staging/post_attachments/a5ab120e28c0902dd0b6237cbf37e05b_5.xlsx",
                        "created_by": 5,
                        "ago": "6d"
                    },
                    {
                        "id": 29,
                        "post_id": 115,
                        "url": "https://s3.amazonaws.com/access_resources/staging/post_attachments/70885aaf0a14ea7bffd55d7aab3ce9b1_5.xls",
                        "created_by": 5,
                        "ago": "6d"
                    },
                    {
                        "id": 30,
                        "post_id": 115,
                        "url": "https://s3.amazonaws.com/access_resources/staging/post_attachments/26a0720678ed43c4ac30bb1650e8e9c1_5.docx",
                        "created_by": 5,
                        "ago": "6d"
                    },
                    {
                        "id": 31,
                        "post_id": 115,
                        "url": "https://s3.amazonaws.com/access_resources/staging/post_attachments/12719a63ff567c8c861ad471f91d5da1_5.doc",
                        "created_by": 5,
                        "ago": "6d"
                    },
                    {
                        "id": 32,
                        "post_id": 115,
                        "url": "https://s3.amazonaws.com/access_resources/staging/post_attachments/b051711347a3260e66cb0f7fa5d261ce_5.pptx",
                        "created_by": 5,
                        "ago": "6d"
                    },
                    {
                        "id": 33,
                        "post_id": 115,
                        "url": "https://s3.amazonaws.com/access_resources/staging/post_attachments/be01a7b8c6fd7b1a9c582d7fc1013e0f_5.ppt",
                        "created_by": 5,
                        "ago": "6d"
                    },
                    {
                        "id": 34,
                        "post_id": 115,
                        "url": "https://s3.amazonaws.com/access_resources/staging/post_attachments/9e40632062858ccdebb05c77f846c6d7_5.png",
                        "created_by": 5,
                        "ago": "6d"
                    },
                    {
                        "id": 35,
                        "post_id": 115,
                        "url": "https://s3.amazonaws.com/access_resources/staging/post_attachments/e99e2b9be0d3d06b8f6011a0221ca241_5.jpg",
                        "created_by": 5,
                        "ago": "6d"
                    },
                    {
                        "id": 36,
                        "post_id": 115,
                        "url": "https://s3.amazonaws.com/access_resources/staging/post_attachments/9a26585c37c7eeb0cbf404489c8da7d5_5.jpeg",
                        "created_by": 5,
                        "ago": "6d"
                    },
                    {
                        "id": 37,
                        "post_id": 115,
                        "url": "https://s3.amazonaws.com/access_resources/staging/post_attachments/825d352c39129209d8464c900b926c97_5.gif",
                        "created_by": 5,
                        "ago": "6d"
                    },
                    {
                        "id": 38,
                        "post_id": 115,
                        "url": "https://s3.amazonaws.com/access_resources/staging/post_attachments/1469c693bbfc2c54ffc622afa6457136_5.mp4",
                        "created_by": 5,
                        "ago": "6d"
                    },
                    {
                        "id": 39,
                        "post_id": 115,
                        "url": "https://s3.amazonaws.com/access_resources/staging/post_attachments/82de00d60acd75cf673a6c943da93c38_5.pdf",
                        "created_by": 5,
                        "ago": "6d"
                    },
                    {
                        "id": 40,
                        "post_id": 115,
                        "url": "https://s3.amazonaws.com/access_resources/staging/post_attachments/1c47518a50241ae73a345750645a14d5_5.mp3",
                        "created_by": 5,
                        "ago": "6d"
                    }
                ]
            },
            "notification": null

        }
    ]
}
```

This requests provides a <strong>HTML 200</strong> on success.