| name          | description                                 | type                   |
|---------------|---------------------------------------------|------------------------|
| id            | The ID of this record                       | integer                |
| name          | The name of this group                      | string                 |
| description   | The description of this group               | string                 |
| owner_user_id | The user ID of the user who owns this group | integer                |
| group_type    | Info about the type of this group           | object; GroupTypeShort |
| owner         | Info about the group owner                  | object; UserShort      |