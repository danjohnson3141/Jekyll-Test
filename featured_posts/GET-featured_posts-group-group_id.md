<!-- --- title: GET /featured_posts/group/:group_id -->

Featured posts are a list of posts that the application displays at the top of several pages (currently: user feed, group feed, event feed). There is no maximum number of posts that will be returned by this route. However, it is possible to artificially limit the number of posts returned through a suffix on the route, which is: '?limit=X' where X is the number to return.

The database table that manages this route only has two relevant fields that are addressed by the application, they are 'post_id' and 'created_at'. The post_id is just the reference to the post that should appear in the feed, created_at is only relevant for purposes of sorting the list.

This particular route returns all of the featured posts that reference the group_id passed in.

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

=
####Response Data Detail:

[[include:/serializers/group_featured_post]]