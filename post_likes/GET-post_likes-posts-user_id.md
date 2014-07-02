<!-- --- title: GET /post_likes/posts/:user_id -->

Retuns **all** of the post likes for **one** users.

=
####Authentication::

The user needs to be logged in and have valid credentials to use this route.

=
####Parameters::

:user_id - Integer, passed in through the URL. Is derived from the 'id' field on the 'users' table.

=
####Response:

This requests provides a <strong>HTML 200</strong> on success.

=
####API request example:
```html
http://example.com/post_likes/posts/27461
```

=
####JSON response example:

[[include:/json/JSON_GET_post_likes_posts_user_id]]

=
####Response Data Detail:

[[include:/serializers/EXAMPLE]]