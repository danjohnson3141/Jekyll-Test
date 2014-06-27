<!-- --- title: DELETE /post_attachments/:id -->

This route removes **one** post_attachment from the database. The active user has to 

=
####Authentication:

The user needs to be logged in and have valid credentials to use this route.

=
####Parameters:

:id (post_comments) - Integer, passed in the URL. Is derived from the 'id' field on the 'post_attachments' table.

=
####Response:

This requests provides a <strong>HTML 204</strong> on success.

=
####API request example:
```html
http://example.com/ROUTE_NAME
```Ï