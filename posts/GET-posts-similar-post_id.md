<!-- --- title: GET /posts/similar/:post_id -->

Returns a list of posts that are associated in someway with the post passed in. The exact functionality of how this is figured out is still in development.

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
http://example.com/posts/similar/12
```

=
####JSON response example:

[[include:/json/JSON_GET_posts_similar_post_id]]

=
####Response Data Detail:

[[include:/serializers/post_feed]]