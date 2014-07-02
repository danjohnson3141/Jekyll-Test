<!-- --- title: GET /post_comments/post/:post_id -->

Returns **all** comments associated with **one** post.

=
####Authentication:

The user needs to be logged in and have valid credentials to use this route.

=
####Parameters:

(post) :id - Integer, passed in through the URL. Is derived from the 'id' field on the 'posts' table.

=
####Response:

This requests provides a <strong>HTML 200</strong> on success.

=
####API request example:
```html
http://example.com/post_comments/post/3758
```

=
####JSON response example:

[[include:/json/JSON_GET_post_comments_post_post_id]]

=
####Response Data Detail:

[[include:/serializers/EXAMPLE]]