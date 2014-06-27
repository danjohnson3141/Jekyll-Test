<!-- --- title: POST /post_attachments -->

This route allows the active user to add an attachment to a post. However, we're not storing the attachment locally, the database is just recording the URL of the file (hosted externally). The active user needs to be the creator of the post that the attachment is being created for.

=
####Authentication:

The user needs to be logged in and have valid credentials to use this route.

=
####Parameters:

None; default only

=
####Response:

This requests provides a <strong>HTML 201</strong> on success.

=
####API request example:
```html
http://example.com/post_attachments
```

=
####Post data example:
```
 { post_attachment: 
 	{ post_id: @post_event_open_mine.id, 
 	  url: 'my_attachment.com', 
 	  attachment_type: @attachment_type.key } }
```
 
=
###Post data detail:

[[include:/post_data/post_post_attachments]]

=
####JSON response example:

[[include:/json/JSON_POST_post_attachments]]

=
####Response Data Detail:

[[include:/serializers/post_attachment]]