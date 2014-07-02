<!-- --- title: GET /event_sessions/event/:event_id -->

Returns **all** of the sessions for **one** event.

=
####Authentication:

The user needs to be logged in and have valid credentials to use this route.

=
####Parameters:

:event_id - Integer, passed in through the URL. Is derived from the 'event_id' field on the 'event_sessions' table.

=
####Response:

This requests provides a <strong>HTML 200</strong> on success.

=
####API request example:
```html
http://example.com/event_sessions/events/5363
```

=
####JSON response example:

[[include:/json/JSON_GET_event_sessions_event_event_id]]

=
####Response Data Detail:

[[include:/serializers/EXAMPLE]]