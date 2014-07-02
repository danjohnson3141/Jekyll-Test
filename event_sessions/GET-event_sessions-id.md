<!-- --- title: GET /event_sessions/:id -->

Returns all the details for one event session.

=
####Authentication:

The user needs to be logged in and have valid credentials to use this route.

=
####Parameters:

:id (event_session)- Integer, passed in through the URL. Derived from the 'id' field from the event_session table.

=
####Response:

This requests provides a <strong>HTML 200</strong> on success.

=
####API request example:
```html
http://example.com/event_sessions/558
```

=
####JSON response example:

[[include:/json/JSON_GET_event_notes_id]]

=
####Response Data Detail:

[[include:/serializers/EXAMPLE]]