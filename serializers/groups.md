| id                        | The id of the group                                                              | integer                 |
|---------------------------|----------------------------------------------------------------------------------|-------------------------|
| name                      | The name of the group                                                            | string                  |
| description               | The description of the group                                                     | string                  |
| owner_user_id             | The ID of the user that owns this group                                          | integer                 |
| member_count              | How many members this group has                                                  | integer                 |
| group_member_id           | The ID of active users group_member record for this group; if it exists          | integer                 |
| group_request_id          | The ID of the active users group_request record for this group; if it exists     | integer                 |
| group_request_is_approved | Whether a group request for this group has been approved                         | boolean                 |
| group_invite_id           | The ID of the group_invite record for this user and group                        | integer                 |
| create_post               | Whether the user can create posts                                                | boolean                 |
| leave_group               | Whether the user can leave the group                                             | boolean                 |
| hide_app_sponsors?        | Whether the app level sponsors should be displayed                               | boolean                 |
| group_type                | Object describing details of the group                                           | object; GroupType       |
| owner                     | User object about the owner of group; uses UserShort                             | object                  |
| group_sponsors            | List of sponsors associated with this group                                      | array                   |
| group_members             | List of group members; uses GroupMemberUser serializer                           | array                   |
| group_invites             | List of pending group_invites for this group; only shows if user is group owner  | array; GroupInviteUser  |
| group_requests            | List of pending group_requests for this group; only shows if user is group owner | array; GroupRequestUser |