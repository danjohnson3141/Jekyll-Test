<!-- --- title: GET /featured_posts/group/:group_id -->

This route returns the featured posts for **one** group.

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
http://stage-api-access.evant.com/group_featured_posts/764
```

=
####JSON response example:

Returns an array of featured_post objects

[[include:/json/JSON_GET_featured_posts_group_group_id]]

####Response Data Detail:

[[include:/serializers/group_featured_post]]