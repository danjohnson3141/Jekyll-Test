<!-- --- title: DELETE /post_likes/:id -->

Removes the like record associated with a post. This is action of 'unliking' a post.

=
####Authentication:

The user needs to be logged in and have valid credentials to use this route.

=
####Parameters:

(post likes) :id - Integer, passed in through the URL. Is derived from the 'id' field on the 'post_likes' table.

=
####API request example:
```json
http://stage-api-access.evant.com/post_likes/234
```

=
####JSON response example:

```json
NO JSON RESPONSE
```

This requests provides a <strong>HTML 204</strong> on success.