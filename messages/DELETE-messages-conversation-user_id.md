<!-- --- title: DELETE /messages/conversation/:user_id -->

This route changes the 'sender_deleted' or 'recipient_deleted' flags on all of the messages between the active user and one other user from 0 to 1. Messages are never actually deleted, just invisibly archived.

=
#### Authentication

The user needs to be logged in and have valid credentials to use this route.

=
#### Parameters

:user_id - Integer, passed in through the URL. Is derived from the 'id' field on the 'users' table.

=
####JSON request example:
```json
http://0.0.0.0:3000/messages/conversation/234
```

=
####JSON response example:

```json
NO JSON RESPONSE
```

This requests provides a <strong>HTML 204</strong> on success.