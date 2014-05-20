| name             | description                                               | type                        |
|------------------|-----------------------------------------------------------|-----------------------------|
| id               | The ID of this record                                     | integer                     |
| body             | Content of the post                                       | string                      |
| is_viewed        | Whether the active user has previously viewed this        | boolean                     |
| post_id          | The ID of the post                                        | integer                     |
| group_id         | The ID of the group                                       | integer                     |
| group_invite_id  | The ID the group invite                                   | integer                     |
| group_request_id | The ID of the group request                               | integer                     |
| ago              | How long ago this was created                             | string                      |
| user             | Info on the user                                          | object; UserTiny            |
| event            | Info on the event                                         | object; EventTiny           |
| user_connection  | Info on the connection between active user and other user | object; UserConnectionShort |