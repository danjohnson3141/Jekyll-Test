<!-- --- title: GET /users/profile/:id -->

This brings back **one** user's profile.

=
#### Authentication

The user needs to be logged in and have valid credentials to use this route.

=
#### Parameters

:user_id - Integer, passed in through the URL. Is derived from the 'id' field on the 'users' table. This the profile that will be returned.

=
####JSON request example:
```json
http://stage-api-access.evant.com/users/profile/1
```

=
####JSON response example:

```json
{
    "user": {
        "id": 1,
        "email": null,
        "alt_email": null,
        "first_name": "Evanta",
        "last_name": "Access",
        "title": "Administrator",
        "organization_name": "Evanta",
        "bio": "System Administrator Account",
        "photo": "https://evanta.com/Resources/contacts/large/91745.jpg",
        "can_message": true,
        "user_role_id": 1,
        "user_connections_blocked": false,
        "post_count": 5,
        "post_like_count": 0,
        "user_connection_count": 7,
        "user_profile": true,
        "can_edit_profile": false,
        "app_language": {
            "id": 1,
            "name": "en",
            "description": "United State English - Native Default Language"
        },
        "connection_status": {
            "id": 6,
            "is_approved": true,
            "is_approver": true
        },
        "event_notes": [],
        "groups": [
            {
                "id": 4,
                "name": "2014 Chicago CIO Executive Summit",
                "group_type_name": "Open"
            },
            {
                "id": 1,
                "name": "CIO",
                "group_type_name": "Open"
            },
            {
                "id": 5,
                "name": "Private Boardroom",
                "group_type_name": "Private"
            }
        ],
        "attended_events": [
            {
                "id": 8,
                "name": "2014 NYC CIO ES"
            }
        ]
    }
}
```

This requests provides a <strong>HTML 200</strong> on success.