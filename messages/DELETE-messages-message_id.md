<!-- --- title: DELETE /messages/:id -->

This route changes the 'sender_deleted' or 'recipient_deleted' flags on *one* message from 0 to 1. Messages are never actually deleted, just invisibly archived.

=
#### Authentication

The user needs to be logged in and have valid credentials to use this route.

=
#### Parameters

:message_id - Integer, passed in through the URL. Is derived from the 'id' field of the 'messages' table.

=
####API request example:
```json
http://stage-api-access.evant.com/messages/123
```

=
####JSON response example:

```json
NO JSON RESPONSE
```

This requests provides a <strong>HTML 204</strong> on success.