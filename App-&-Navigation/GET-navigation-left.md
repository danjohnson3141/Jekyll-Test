<!-- --- title: GET /navigation/left -->

This is a route to help populate the left navigation element in the app (e.g. clicking on the bug).

The 'user_today_events' field of the json only returns events that the user is registered for or is attending. This comes off of the 'event_registration_status_id' field of the 'event_users' table.

=
#### Authentication

The user needs to be logged in and have valid credentials to use this route.

#### Parameters

This route has no parameters and returns its content based on the users's internal settings.

=
####API request example:
```json
http://stage-api-access.evant.com/navigation/left
```
=
####JSON response example:

```json
{
    "navigation_left": {
        "show_messages": true,
        "show_notifications": true,
        "show_search": true,
        "show_user_profile": true,
        "show_posts_count": true,
        "show_likes_count": true,
        "show_connections_count": true,
        "show_groups": true,
        "show_events": true,
        "show_app_sponsors": true,
        "show_support_link": true,
        "new_message_count": 0,
        "new_notification_count": 162,
        "user_headshot": "https://s3.amazonaws.com/access_resources/staging/thumbnails/7.jpg?12",
        "user_full_name": "Graham Baas",
        "user_title": "Quality Assurance",
        "user_organization": "Evanta",
        "user_post_count": 18,
        "user_like_count": 6,
        "user_connection_count": 4,
        "user_pending_connection_count": 0,
        "user_events": [
            {
                "id": 7,
                "name": "2015 HOU CIO ES"
            },
            {
                "id": 9,
                "name": "2015 BOS CISO ES ZQZQ"
            },
            {
                "id": 8,
                "name": "2014 NYC CIO ES"
            }
        ],
        "user_today_events": [],
        "user_groups": [
            {
                "id": 7,
                "name": "Test_Secret",
                "group_type_name": "Secret"
            },
            {
                "id": 8,
                "name": "Test_Public",
                "group_type_name": "Open"
            },
            {
                "id": 9,
                "name": "Test_Private",
                "group_type_name": "Private"
            }
        ]
    }
}
```

This requests provides a **HTML 200** on success.