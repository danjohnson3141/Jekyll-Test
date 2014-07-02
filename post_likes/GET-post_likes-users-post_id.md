<!-- --- title: GET /post_likes/users/:post_id -->

Returns **all** post likes for **one** post.

=
####Authentication:

The user needs to be logged in and have valid credentials to use this route.

=
####Parameters:

:post_id - Integer, passed in through the URL. Is derived from the 'id' field on the 'posts' table.

=
####Response:

This requests provides a <strong>HTML 200</strong> on success.

=
####API request example:
```html
http://example.com/post_likes/user/2304
```

=
####JSON response example:

[[include:/json/JSON_NEEDS_EXAMPLE]]

=
####Response Data Detail:

[[include:/serializers/EXAMPLE]]