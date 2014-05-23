<!-- --- title: GET /users/profile -->

This route shows the profile for the active user. This route returns a lot of information about the user.

=
####Authentication:

The user needs to be logged in and have valid credentials to use this route.

=
####Parameters:

none; defaults only

=
####API request example:
```html
http://stage-api-access.evant.com/users/profile
```

=
####JSON response example:

```json
{
    "user": {
        "id": 7,
        "email": "graham.baas@evanta.com",
        "alt_email": "bad@example.com",
        "first_name": "Graham",
        "last_name": "Baas",
        "title": "Quality Assurance",
        "organization_name": "Evanta",
        "bio": "Tester Extraordinaire",
        "photo": "https://s3.amazonaws.com/access_resources/staging/thumbnails/7.jpg?12",
        "can_message": false,
        "user_role_id": 1,
        "user_connections_blocked": false,
        "post_count": null,
        "post_like_count": 5,
        "user_connection_count": 4,
        "user_profile": true,
        "can_edit_profile": true,
        "app_language": {
            "id": 3,
            "name": "fr",
            "description": "French (Français)"
        },
        "connection_status": null,
        "event_notes": [],
        "groups": [
            {
                "id": 4,
                "name": "2014 Chicago CIO Executive Summit",
                "group_type_name": "Open"
            },
            {
                "id": 3,
                "name": "CDO",
                "group_type_name": "Open"
            },
            {
                "id": 1,
                "name": "CIO",
                "group_type_name": "Open"
            },
            {
                "id": 2,
                "name": "CISO",
                "group_type_name": "Open"
            },
            {
                "id": 15,
                "name": "Dan's cool group",
                "group_type_name": "Open"
            },
            {
                "id": 14,
                "name": "RELEASE THE BRAKKEN!!!",
                "group_type_name": "Private"
            },
            {
                "id": 9,
                "name": "Test_Private",
                "group_type_name": "Private"
            },
            {
                "id": 8,
                "name": "Test_Public",
                "group_type_name": "Open"
            },
            {
                "id": 7,
                "name": "Test_Secret",
                "group_type_name": "Secret"
            }
        ],
        "attended_events": [
            {
                "id": 1,
                "name": "2014 HOU CIO ES"
            },
            {
                "id": 3,
                "name": "2014 BOS CISO ES"
            }
        ]
    }
}
```

This requests provides a <strong>HTML 200</strong> on success.