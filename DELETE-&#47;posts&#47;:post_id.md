This deletes a post. Only the user that created the post is allowed to delete the post.

=
#### Authentication

The user needs to be logged in and have valid credentials to use this route.

=
#### Parameters

:post_id - Integer, passed in through the URL. Used to declare which post is going to be updated. It is derived from the 'id' field on the 'posts' table.

=
####JSON request example:
```
http://0.0.0.0:3000/ROUTE_NAME
```

=
####JSON response example:

```
NO JSON RESPONSE
```

This requests provides a <strong>HTML 204</strong> on success.