<!-- --- title: DELETE /user_connections/:id -->

This route deletes a user connection. The user is only able to delete connections that they are a part of (either sender or recipient), if they are the recipient they are able to delete it before it is approved. If they are the sender, the user is not allowed to delete the record until it's been approved by the recipient.
 
=
#### Authentication

The user needs to be logged in and have valid credentials to use this route.

=
#### Parameters

:user_connection_id - Integer, passed in through the URL. Is derived from the 'id' field on the 'user_connection' table.

=
####JSON request example:
```json
http://0.0.0.0:3000/user_connections/234
```

=
####JSON response example:

```json
NO JSON RESPONSE
```

This requests provides a <strong>HTML 204</strong> on success.