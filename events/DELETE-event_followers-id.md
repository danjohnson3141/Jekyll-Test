<!-- --- title: DELETE /event_followers/:id -->

This is how a user unfollows an events.

=
#### Authentication

The user needs to be logged in and have valid credentials to use this route.

=
#### Parameters

:id - Integer, passed in through the URL. Is derived from the 'id' field on the 'event_followers' table.

=
####API request example:
```json
http://stage-api-access.evant.com/event_followers/234
```

=
####JSON response example:

```json
NO JSON RESPONSE
```

This requests provides a <strong>HTML 204</strong> on success.