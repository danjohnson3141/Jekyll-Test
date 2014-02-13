This route changes the 'sender_deleted' or 'recipient_deleted' flags on messages from 0 to 1. Messages are never actually deleted, just invisibly archived.

=
#### Authentication

The user needs to be logged in and have valid credentials to use this route.

=
#### Parameters

/:id

Passed in the URL, id number is derived from the 'id' field of the 'messages' table.

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