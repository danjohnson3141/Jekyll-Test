<!-- --- title: PATCH /post_comments/:id -->

Allows the active user to edit the content of **one** post comment.

=
#### Authentication

The user needs to be logged in and have valid credentials to use this route.

=
#### Parameters

:body - Text, passed in through the post data. This is the plain text of the submission.

(post comment) :id - Integer, passed in through the URL. Is derived from the 'id' field on the 'post_comments' table.

=
####API request example:
```json
http://stage-api-access.evant.com/post_comments/234
```

=
####Post Data
```
{ post_comment: { body: 'This is the updated body of the post_comment.' } }
```

=
####JSON response example:

```json
NO JSON RESPONSE
```

This requests provides a <strong>HTML 204</strong> on success.