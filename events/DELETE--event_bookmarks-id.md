<!-- --- title: DELETE /event_bookmarks/:id -->

Removes one specific event bookmark for the user.

=
#### Authentication

The user needs to be logged in and have valid credentials to use this route.

=
#### Parameters

:id - Integer, passed in through the URL. Is derived from the 'id' field on the 'event_bookmarks' table.

=
####JSON request example:
```json
http://0.0.0.0:3000/event_bookmarks/234
```

=
####JSON response example:

```json
NO JSON RESPONSE
```

This requests provides a <strong>HTML 204</strong> on success.