<!-- --- title: GET /featured_posts/group/:group_id -->

Featured posts are a list of posts that the application displays at the top of several pages (currently: user feed, group feed, event feed). There is no maximum number of posts that will be returned by this route. However, it is possible to artificially limit the number of posts returned through a suffix on the route, which is: '?limit=X' where X is the number to return.

The database table that manages this route only has two relevant fields that are addressed by the application, they are 'post_id' and 'created_at'. The post_id is just the reference to the post that should appear in the feed, created_at is only relevant for purposes of sorting the list.

This particular route returns all of the featured posts that reference the group_id passed in.

=
#### Authentication

The user needs to be logged in and have valid credentials to use this route.

=
#### Parameters

:group_id - Integer, passed in through the URL. Is derived from the 'group_id' field on the 'featured_posts' table.

=
####JSON request example:
```json
http://stage-api-access.evant.com/featured_posts/group/1?limit=5
```

=
####JSON response example:

```json
{
    "featured_posts": [
        {
            "id": 10,
            "post": {
                "id": 18,
                "title": null,
                "excerpt": null,
                "generated_excerpt": "Voluptas ut itaque inventore eos sit ipsum ut. Architecto quia neque non. Unde explicabo sunt fuga. Deserunt voluptate odio.\n\nDolores sequi iste nostrum. Et impedit dolores aspernatur facere officia e",
                "body": "Voluptas ut itaque inventore eos sit ipsum ut. Architecto quia neque non. Unde explicabo sunt fuga. Deserunt voluptate odio.\n\nDolores sequi iste nostrum. Et impedit dolores aspernatur facere officia et. Ut placeat adipisci molestias doloribus doloremque nemo excepturi.",
                "body_markdown": null,
                "thumbnail_teaser_photo": "http://placekitten.com/320/500",
                "display_rank": 6,
                "view_count": 4,
                "like_count": 2,
                "can_like": true,
                "comment_count": 0,
                "can_comment": true,
                "can_delete": false,
                "post_like_id": null,
                "ago": "15d",
                "event_session_id": null,
                "created_by": 9,
                "group": {
                    "id": 1,
                    "name": "CIO",
                    "group_type_name": "Open"
                },
                "event": null,
                "sponsor": null,
                "authors": [
                    {
                        "id": 9,
                        "first_name": "Adam",
                        "last_name": "Lorts",
                        "title": "Dev Now Consultant",
                        "organization_name": "Development Now",
                        "photo": "https://s3.amazonaws.com/access_resources/staging/thumbnails/9.jpg?17",
                        "moderator": false,
                        "user_profile": true
                    }
                ],
                "post_attachments": [
                    {
                        "id": 5,
                        "post_id": 18,
                        "url": "https://www.attachment.com/attachment",
                        "created_by": 10,
                        "ago": "13d"
                    }
                ],
                "post_comments": []
            }
        },
        {
            "id": 7,
            "post": {
                "id": 4,
                "title": "Fundamental intermediate intranet: Practical Cotton Shirt",
                "excerpt": "Vel occaecati quae temporibus omnis. Consequatur et ea.\n\nConsequatur animi est ratione quam voluptatum quos. Perspiciatis repudiandae et aliquam. Debitis consequatur minus.",
                "generated_excerpt": "Vel occaecati quae temporibus omnis. Consequatur et ea.\n\nConsequatur animi est ratione quam voluptatum quos. Perspiciatis repudiandae et aliquam. Debitis consequatur minus.",
                "body": "Vel occaecati quae temporibus omnis. Consequatur et ea.\n\nConsequatur animi est ratione quam voluptatum quos. Perspiciatis repudiandae et aliquam. Debitis consequatur minus.",
                "body_markdown": null,
                "thumbnail_teaser_photo": "http://placekitten.com/250/250",
                "display_rank": 4,
                "view_count": 44,
                "like_count": 1,
                "can_like": true,
                "comment_count": 3,
                "can_comment": true,
                "can_delete": false,
                "post_like_id": null,
                "ago": "17d",
                "event_session_id": null,
                "created_by": 6,
                "group": {
                    "id": 1,
                    "name": "CIO",
                    "group_type_name": "Open"
                },
                "event": null,
                "sponsor": {
                    "id": 3,
                    "name": "Volkman Group",
                    "description": "Customer-focused local analyzer",
                    "logo": "https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTvGG2FajNhzpotZNYL1pjD7bLbAdZZMahlCrPrPyozfoZ61etV_Q",
                    "url": "http://rippin.biz/danny.grant",
                    "event_note_id": null,
                    "event_bookmark_id": null,
                    "sponsor_type": {
                        "id": 2,
                        "name": "Enterprise Sponsor",
                        "description": "Multi-layered secondary conglomeration",
                        "display_rank": 20
                    },
                    "banner_ads": [
                        {
                            "id": 7,
                            "graphic_link": "http://placehold.it/840x100/bacf8b/ffffff/&text=[Sponsor:+3,+Banner:+7]",
                            "link_url": "www.evanta.com"
                        },
                        {
                            "id": 8,
                            "graphic_link": "http://placehold.it/840x100/d6f53c/ffffff/&text=[Sponsor:+3,+Banner:+8]",
                            "link_url": "www.evanta.com"
                        },
                        {
                            "id": 9,
                            "graphic_link": "http://placehold.it/840x100/e4d600/ffffff/&text=[Sponsor:+3,+Banner:+9]",
                            "link_url": "www.evanta.com"
                        }
                    ]
                },
                "authors": [
                    {
                        "id": 6,
                        "first_name": "Brittany",
                        "last_name": "Budil",
                        "title": "Project Manager",
                        "organization_name": "Evanta",
                        "photo": "https://s3.amazonaws.com/access_resources/staging/thumbnails/6.jpg?43",
                        "moderator": false,
                        "user_profile": true
                    }
                ],
                "post_attachments": [],
                "post_comments": [
                    {
                        "id": 2,
                        "body": "Repellendus doloribus dolore hic iusto quos.\n\nQui perferendis itaque. Ratione placeat ipsum doloribus unde qui. Voluptas excepturi qui necessitatibus aut placeat.",
                        "ago": "16d",
                        "creator": {
                            "id": 13,
                            "first_name": "Shyanne",
                            "last_name": "Weimann",
                            "title": "VP, Business Development",
                            "organization_name": "Accenture",
                            "photo": "https://evanta.com/Resources/contacts/large/92083.jpg",
                            "moderator": false,
                            "user_profile": true
                        }
                    },
                    {
                        "id": 10,
                        "body": "Odio cum quis.\n\nDeleniti beatae impedit quo consequuntur quae. Repellendus voluptas quo qui non ducimus ab nobis. Debitis harum necessitatibus dolorem nostrum illo.",
                        "ago": "15d",
                        "creator": {
                            "id": 27,
                            "first_name": "Hermina",
                            "last_name": "Reichert",
                            "title": "Random User",
                            "organization_name": "Brown, Monahan and Abbott",
                            "photo": "https://s3.amazonaws.com/access_resources/staging/thumbnails/27.jpg?33",
                            "moderator": false,
                            "user_profile": true
                        }
                    },
                    {
                        "id": 20,
                        "body": "Iste ut minus quia est perferendis in.\n\nVoluptatem iste velit vero deleniti. Quasi maiores quia commodi. Quis aspernatur omnis. Corrupti similique animi consequatur voluptates.",
                        "ago": "17d",
                        "creator": {
                            "id": 21,
                            "first_name": "Dena",
                            "last_name": "Kuhlman",
                            "title": "Chief Information Officer",
                            "organization_name": "Kilback and Sons",
                            "photo": "https://s3.amazonaws.com/access_resources/staging/thumbnails/21.jpg?17",
                            "moderator": false,
                            "user_profile": true
                        }
                    }
                ]
            }
        }
    ]
}

```

This requests provides a <strong>HTML 200</strong> on success.