<!-- --- title: GET /event_notes/event/:event_id -->

Returns **all** of the active user's event notes for **one** event.

=
####Authentication:

The user needs to be logged in and have valid credentials to use this route.

=
####Parameters:

:event_id - Integer, passed in through the URL. Is derived from the 'id' field of the 'events' table.

=
####Response:

This requests provides a <strong>HTML 200</strong> on success.

=
####API request example:
```html
http://example.com/event_notes/event/6038
```

=
####JSON response example:

[[include:/json/JSON_GET_event_notes_event_event_id]]

=
####Response Data Detail:

[[include:/serializers/event_note]]