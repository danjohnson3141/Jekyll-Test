<!-- --- title: DELETE /post_comments/:id -->

Deletes *one* comment that exists associated with a post.

=
#### Authentication

The user needs to be logged in and have valid credentials to use this route.

=
#### Parameters

(post comment) :id - Integer, passed in throug the URL. Is derived form the 'id' field on the 'post_comments' table.

=
####JSON request example:
```json
http://0.0.0.0:3000/post_comments/234
```

=
####JSON response example:

```json
NO JSON RESPONSE
```

This requests provides a <strong>HTML 204</strong> on success.