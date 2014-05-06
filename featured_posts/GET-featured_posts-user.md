<!-- --- title: GET /featured_posts/user -->

Featured posts are a list of posts that the application displays at the top of several pages (currently: user feed, group feed, event feed). There is no maximum number of posts that will be returned by this route. However, it is possible to artificially limit the number of posts returned through a suffix on the route, which is: '?limit=X' where X is the number to return.

The database table that manages this route only has two relevant fields that are addressed by the application, they are 'post_id' and 'created_at'. The post_id is just the reference to the post that should appear in the feed, created_at is only relevant for purposes of sorting the list.

The user route (as opposed to event and group routes) is composed of all the featured group posts from groups that the active user is a member of.

=
#### Authentication

Declare what authentications are required
Good sample text: The user needs to be logged in and have valid credentials to use this route.

=
#### Parameters

suffix: '?limit=X' 

=
####JSON request example:
```json
http://0.0.0.0:3000/featured_posts/user?limit=5
```

=
####JSON response example:

```json
{
    "featured_posts": [
        {
            "id": 13,
            "post": {
                "id": 20,
                "title": null,
                "excerpt": null,
                "generated_excerpt": "Totam et autem. Explicabo eos eum soluta culpa quos ut nihil.\n\nEnim quas aut ullam eaque. Quo incidunt eius sequi consequatur aut porro magni. Ut sed est dolor.",
                "body": "Totam et autem. Explicabo eos eum soluta culpa quos ut nihil.\n\nEnim quas aut ullam eaque. Quo incidunt eius sequi consequatur aut porro magni. Ut sed est dolor.",
                "body_markdown": null,
                "thumbnail_teaser_photo": "http://placekitten.com/250/320",
                "display_rank": 3,
                "view_count": 23,
                "like_count": 1,
                "can_like": true,
                "comment_count": 2,
                "can_comment": true,
                "can_delete": false,
                "post_like_id": null,
                "ago": "19d",
                "event_session_id": null,
                "created_by": 5,
                "group": {
                    "id": 4,
                    "name": "2014 Chicago CIO Executive Summit",
                    "group_type_name": "Open"
                },
                "event": null,
                "sponsor": null,
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
                        "id": 6,
                        "post_id": 20,
                        "url": "https://www.attachment.com/attachment",
                        "created_by": 25,
                        "ago": "13d"
                    }
                ],
                "post_comments": [
                    {
                        "id": 12,
                        "body": "Provident ut ea et ab quaerat aut mollitia.\n\nAlias voluptas et. Officiis ut voluptatum quia natus non excepturi. Illum rerum odio fuga repudiandae omnis non.",
                        "ago": "16d",
                        "creator": {
                            "id": 2,
                            "first_name": "Michael",
                            "last_name": "Irey",
                            "title": "Software Engineer",
                            "organization_name": "Evanta",
                            "photo": "https://s3.amazonaws.com/access_resources/staging/thumbnails/2.jpg?4",
                            "moderator": false,
                            "user_profile": true
                        }
                    },
                    {
                        "id": 56,
                        "body": "123123",
                        "ago": "8d",
                        "creator": {
                            "id": 7,
                            "first_name": "Graham",
                            "last_name": "Baas",
                            "title": "Quality Assurance",
                            "organization_name": "Evanta",
                            "photo": "https://s3.amazonaws.com/access_resources/staging/thumbnails/7.jpg?12",
                            "moderator": false,
                            "user_profile": true
                        }
                    }
                ]
            }
        },
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
            "id": 9,
            "post": {
                "id": 88,
                "title": null,
                "excerpt": null,
                "generated_excerpt": "Deleniti saepe architecto. Aut quidem et vitae accusamus libero. Voluptas beatae qui et rerum excepturi rerum repellendus.\n\nFacere et praesentium minus et asperiores architecto. Quia sint assumenda di",
                "body": "Deleniti saepe architecto. Aut quidem et vitae accusamus libero. Voluptas beatae qui et rerum excepturi rerum repellendus.\n\nFacere et praesentium minus et asperiores architecto. Quia sint assumenda distinctio non. Necessitatibus ab maiores ad aliquid doloribus. Exercitationem qui impedit laudantium. Expedita eos totam ea quia.",
                "body_markdown": null,
                "thumbnail_teaser_photo": "http://placekitten.com/500/500",
                "display_rank": 1,
                "view_count": 3,
                "like_count": 1,
                "can_like": true,
                "comment_count": 1,
                "can_comment": true,
                "can_delete": false,
                "post_like_id": null,
                "ago": "18d",
                "event_session_id": null,
                "created_by": 23,
                "group": {
                    "id": 4,
                    "name": "2014 Chicago CIO Executive Summit",
                    "group_type_name": "Open"
                },
                "event": null,
                "sponsor": {
                    "id": 30,
                    "name": "Accenture",
                    "description": "Accenture is a global management consulting, technology services and outsourcing company, with 257,000 people serving clients in more than 120 countries. Combining unparalleled experience, comprehensive capabilities across all industries and business functions, and extensive research on the world’s most successful companies, Accenture collaborates with clients to help them become high-performance businesses and governments. The company generated net revenues of US$27.9 billion for the fiscal year ended Aug. 31, 2012.",
                    "logo": "https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRGewb1V7HhET93s08W7G0Zv79DQO3o-8X-nSm9jY8fky8cH-h0",
                    "url": "www.accenture.com",
                    "event_note_id": null,
                    "event_bookmark_id": null,
                    "sponsor_type": {
                        "id": 5,
                        "name": "Session Host ",
                        "description": "Virtual tangible strategy",
                        "display_rank": 50
                    },
                    "banner_ads": [
                        {
                            "id": 88,
                            "graphic_link": "https://s3.amazonaws.com/uploads.hipchat.com/16269/786687/gdWPws1FXPWYuWe/QTS.png",
                            "link_url": "www.evanta.com"
                        },
                        {
                            "id": 89,
                            "graphic_link": "https://s3.amazonaws.com/uploads.hipchat.com/16269/786687/oF8YsJ8FWCOctKZ/IBM.png",
                            "link_url": "www.evanta.com"
                        }
                    ]
                },
                "authors": [
                    {
                        "id": 23,
                        "first_name": "Jacques",
                        "last_name": "Heidenreich",
                        "title": "VP, Technology",
                        "organization_name": "McGlynn Group",
                        "photo": "https://s3.amazonaws.com/access_resources/staging/thumbnails/23.jpg?96",
                        "moderator": false,
                        "user_profile": true
                    }
                ],
                "post_attachments": [],
                "post_comments": [
                    {
                        "id": 36,
                        "body": "Nam hic et. Est enim voluptates consectetur.\n\nIn maiores illo voluptatem accusamus. Accusamus omnis quia laboriosam eaque commodi. Voluptas sit id et ut iure.",
                        "ago": "15d",
                        "creator": {
                            "id": 12,
                            "first_name": "Etha",
                            "last_name": "Willms",
                            "title": "CIO",
                            "organization_name": "Heller, Heller and Cronin",
                            "photo": "https://evanta.com/Resources/contacts/large/92034.jpg",
                            "moderator": false,
                            "user_profile": true
                        }
                    }
                ]
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