<!-- --- title: DELETE /event_users/:event_user_id -->

This removes an event_users record. Event_users keeps track of event registrations and their status.

=
####Authentication:

The user needs to be logged in and have valid credentials to use this route.

=
####Parameters:

:event_user_id - Integer, passed in through the URL. Is derived from the 'id' field of the '

=
####API request example:
```json
http://stage-api-access.evant.com/event_users/234
```

=
####JSON response example:

[[include:/json/JSON_NO_RESPONSE]]

This requests provides a <strong>HTML 204</strong> on success.