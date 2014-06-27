| name            | description                                      | type                   |
|-----------------|--------------------------------------------------|------------------------|
| id              | The ID of this record                            | integer                |
| post_id         | The ID of the post                               | integer                |
| url             | The address of where the resource is being hostd | string                 |
| display_rank    | Allows for arbitrary sorting of results          | integer                |
| created_by      | The user_id of the person that creatd the record | integer                |
| ago             | How long ago this was created                    | string                 |
| attachment_type | Info on the file type                            | object; AttachmentType |