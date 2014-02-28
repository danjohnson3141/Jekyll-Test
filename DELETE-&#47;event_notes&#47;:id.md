Removes one event_notes record for the user.

=
#### Authentication

The user needs to be logged in and have valid credentials to use this route.

=
#### Parameters

:id - Integer, passed in through the URL. Is derived from the 'id' field on the 'event_notes' table.

=
####JSON request example:
```
http://0.0.0.0:3000/event_notes/234
```

=
####JSON response example:

```
NO JSON RESPONSE
```

This requests provides a <strong>HTML 204</strong> on success.