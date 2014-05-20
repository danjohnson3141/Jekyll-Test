| name                     | description                                                                            | type                        |
|--------------------------|----------------------------------------------------------------------------------------|-----------------------------|
| id                       | The ID of this record                                                                  | integer                     |
| first_name               | The user's first name                                                                  | string                      |
| last_name                | The user's last name                                                                   | string                      |
| user_connections_blocked | Whether the active user can connect with this user                                     | boolean                     |
| user_profile             | Whether the user has a profile, usually used for speakers who don't have full profiles | boolean                     |
| connection_status        | Info on connection status between this and active user                                 | object; UserConnectionShort |