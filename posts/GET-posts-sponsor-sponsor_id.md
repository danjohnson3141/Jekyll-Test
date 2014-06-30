<!-- --- title: GET /posts/sponsor/:sponsor_id -->

Returns **all** the posts associated with **one** sponsor.

=
####Authentication:

The user needs to be logged in and have valid credentials to use this route.

=
####Parameters:

sponsor_id, The ID of the sponsor, integer 

=
####Response:

This requests provides a <strong>HTML 200</strong> on success.

=
####API request example:
```html
http://example.com/posts/sponsor/4
```

=
####JSON response example:

[[include:/json/JSON_GET_posts_sponsor_sponsor_id]]

=
####Response Data Detail:

[[include:/serializers/post_feed]]