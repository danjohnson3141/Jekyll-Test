| name | description | type
|--------------------------|----------------------------------------------------------------------------------------|-----------------------------|
| alt_email                | The alt email address of this user; should only show if this is active user profile    | string                      |
| app_language             |                                                                                        | object; AppLanguage         |
| attended_events          | The events (visible to the active user) that this user has attended                    | array; AttendedEvent        |
| bio                      | Description of this user                                                               | string                      |
| can_edit_profile         | Whether the active user can edit this profile                                          | boolean                     |
| can_message              | Whether the active user can message this user                                          | boolean                     |
| connection_status        | Info on connection status between this and active user                                 | object; UserConnectionShort |
| email                    | The email address of this user; should only show if this is active user profile        | string                      |
| event_council_member     | Whether this user is an event_council_member for this event                            | boolean                     |
| event_notes              | Any event notes that the active user may have created for this user                    | array; EventNoteShort       |
| first_name               | The user's first name                                                                  | string                      |
| groups                   | The groups (visible to the active user) that this user belongs to                      | array; GroupTiny            |
| id                       | The ID of the user record                                                              | integer                     |
| last_name                | The user's last name                                                                   | string                      |
| name                     | description                                                                            | type                        |
| organization_name        | The organization the user is associated with                                           | string                      |
| photo                    | URL of a photo of the user                                                             | string                      |
| post_count               | How many posts (visible to the active user) this user has created                      | integer                     |
| post_like_count          | How many post likes (visible to the active user) this user has created                 | integer                     |
| title                    | The user's title                                                                       | string                      |
| user_connection_count    | How many connections (visible to the active user) this user has created                | integer                     |
| user_connections_blocked | Whether the active user can connect with this user                                     | boolean                     |
| user_profile             | Whether the user has a profile, usually used for speakers who don't have full profiles | boolean                     |
| user_profile             | Whether the user has a profile, usually used for speakers who don't have full profiles | boolean                     |
| user_role_id             | The ID of this user's role                                                             | integer                     |