<!-- --- title: GET /featured_posts/group/:group_id -->

This route returns all the featured posts for one group.

=
#### Authentication

The user needs to be logged in and have valid credentials to use this route.

=
#### Parameters

:group_id - Integer, passed in through the URL. Is derived from the 'group_id' field on the 'featured_posts' table.

=
####JSON request example:
```json
http://0.0.0.0:3000/featured_posts/event/4316
```

=
####JSON response example:

```json

```

This requests provides a <strong>HTML 200</strong> on success.