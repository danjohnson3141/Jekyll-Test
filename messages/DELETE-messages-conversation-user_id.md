<!-- --- title: DELETE /messages/conversation/:user_id -->

This route changes the 'sender_deleted' or 'recipient_deleted' flags on all of the messages between the active user and one other user from 0 to 1. Messages are never actually deleted, just invisibly archived.

=
####Authentication:

The user needs to be logged in and have valid credentials to use this route.

=
####Parameters:

:user_id - Integer, passed in through the URL. Is derived from the 'id' field on the 'users' table.

=
####Response:

This requests provides a <strong>HTML 204</strong> on success.

=
####API request example:
```json
http://stage-api-access.evant.com/messages/conversation/234
```

=
####JSON response example:

[[include:/json/JSON_NO_RESPONSE]]