<!-- --- title: DELETE /post_likes/:id -->

Removes the like record associated with a post. This is action of 'unliking' a post.

=
####Authentication:

The user needs to be logged in and have valid credentials to use this route.

=
####Parameters:

(post likes) :id - Integer, passed in through the URL. Is derived from the 'id' field on the 'post_likes' table.

=
####Response:

This requests provides a <strong>HTML 204</strong> on success.

=
####API request example:
```html
http://example.com/post_likes/234
```

=
####JSON response example:

[[include:/json/JSON_NO_RESPONSE]]