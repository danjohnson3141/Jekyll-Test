<!-- --- title: GET /event_notes/:id -->

Returns **one** event note based on the data passed in.

=
####Authentication:

The user needs to be logged in and have valid credentials to use this route.

=
####Parameters:

(event_notes) :id - Integer, passed in through the URL. Is derived from the 'id' field of the 'event_notes' table.

=
####Response:

This requests provides a <strong>HTML 200</strong> on success.

=
####API request example:
```html
http://example.com/event_notes/14
```

=
####JSON response example:

[[include:/json/JSON_GET_event_notes_id]]

=
####Response Data Detail:

[[include:/serializers/event_note_short]]