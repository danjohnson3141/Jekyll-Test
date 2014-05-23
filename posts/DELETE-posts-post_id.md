<!-- --- title: DELETE /posts/:id -->

This deletes a post. Only the user that created the post is allowed to delete the post.

=
####Authentication:

The user needs to be logged in and have valid credentials to use this route.

=
####Parameters:

:post_id - Integer, passed in through the URL. Used to declare which post is going to be updated. It is derived from the 'id' field on the 'posts' table.

=
####API request example:
```html
http://stage-api-access.evant.com/posts/234
```

=
####JSON response example:

[[include:/json/JSON_NO_RESPONSE]]

This requests provides a <strong>HTML 204</strong> on success.