<!-- --- title: GET /posts/group/:group_id -->

This returns **all** the posts associated with one group.

=
####Authentication:

The user needs to be logged in and have valid credentials to use this route.

=
####Parameters:

:group_id - Integer, passed in through the URL. Is derived from the 'id' field on the 'groups' table.

=
####Response:

This requests provides a <strong>HTML 200</strong> on success.

=
####API request example:
```json
http://stage-api-access.evant.com/posts/groups/2197
```

=
####JSON response example:

Returns an array of 

[[include:/json/JSON_GET_posts_group_group_id]]

=
####Response Data Detail:

[[include:/serializers/post_feed]]