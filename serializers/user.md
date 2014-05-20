| name                     | description                                                                            | type                        |
|--------------------------|----------------------------------------------------------------------------------------|-----------------------------|
| id                       | The ID of the user record                                                              | integer                     |
| email                    | The email address of this user; should only show if this is active user profile        | string                      |
| alt_email                | The alt email address of this user; should only show if this is active user profile    | string                      |
| first_name               | The user's first name                                                                  | string                      |
| last_name                | The user's last name                                                                   | string                      |
| title                    | The user's title                                                                       | string                      |
| organization_name        | The organization the user is associated with                                           | string                      |
| bio                      | Description of this user                                                               | string                      |
| photo                    | URL of a photo of the user                                                             | string                      |
| can_message              | Whether the active user can message this user                                          | boolean                     |
| user_role_id             | The ID of this user's role                                                             | integer                     |
| user_connections_blocked | Whether the active user can connect with this user                                     | boolean                     |
| post_count               | How many posts (visible to the active user) this user has created                      | integer                     |
| post_like_count          | How many post likes (visible to the active user) this user has created                 | integer                     |
| user_connection_count    | How many connections (visible to the active user) this user has created                | integer                     |
| user_profile             | Whether the user has a profile, usually used for speakers who don't have full profiles | boolean                     |
| can_edit_profile         | Whether the active user can edit this profile                                          | boolean                     |
| app_language             | Info on the language setting chosen by this user                                       | object; AppLanguage         |
| connection_status        | Info on connection status between this and active user                                 | object; UserConnectionShort |
| event_notes              | Any event notes that the active user may have created for this user                    | array; EventNoteShort       |
| groups                   | The groups (visible to the active user) that this user belongs to                      | array; GroupTiny            |
| attended_events          | The events (visible to the active user) that this user has attended                    | array; AttendedEvent        |