| name                   | description                                                                                       | type                      |
|------------------------|---------------------------------------------------------------------------------------------------|---------------------------|
| id                     | The ID of the post being referenced                                                               | integer                   |
| title                  | The title of the post                                                                             | string                    |
| excerpt                | The lede of the post; is user defined                                                             | string                    |
| generated_excerpt      | The first 200 characters of the body; only present if excerpt is not defined                      | string                    |
| thumbnail_teaser_photo | Link to a small teaser photo                                                                      | string                    |
| view_count             | How many users have viewed this post                                                              | integer                   |
| show_likes_count?      | Whether to show the likes count                                                                   | boolean                   |
| like_count             | How many users have liked this post                                                               | integer                   |
| comment_count          | How many comments are on this post                                                                | integer                   |
| post_like_id           | If the user has liked this post; the ID of that post                                              | integer                   |
| can_like?              | Whether the user is able to like this post                                                        | boolean                   |
| featured?              | Whether this post is a featured post                                                              | boolean                   |
| show_post_likes_list?  | Whether to show the list of users who have liked this post                                        | boolean                   |
| ago                    | How long ago this post was created                                                                | string                    |
| created_by             | The ID of the user that created this post                                                         | integer                   |
| group                  | The group associated with this post (has to be either group, event, or event_session)             | object; GroupTiny         |
| event                  | The event associated with this post (has to be either group, event, or event_session)             | object; EventTinys        |
| sponsor                | The sponsor associated with this post                                                             | object; SponsorTiny       |
| event_session          | The event_session associated with this post (has to be either group, event, or event_session)     | object; EventSessionMicro |
| recent_activity        | The most recent action taken on this post (like, comment, add attachment)                         | object; Recent Activity   |
| authors                | The user that created this post or users associated to this post through post_contributor records | array; UserTiny           |
| post_attachments       | The attachments associated with this post                                                         | array; PostAttachment     |