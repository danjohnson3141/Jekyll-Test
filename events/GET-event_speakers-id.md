<!-- --- title: GET /event_speakers/:id -->

Returns information for one event speaker.

=
####Authentication:

The user needs to be logged in and have valid credentials to use this route.

=
####Parameters:

:id (event_speaker) - Integer, passed in through the URL. Is derived from the 'id' field on the 'event_speaker' table.

=
####Response:

This requests provides a <strong>HTML 200</strong> on success.

=
####API request example:
```html
http://example.com/event_speakers/61
```

=
####JSON response example:

[[include:/json/JSON_GET_event_speakers_id]]

=
####Response Data Detail:

[[include:/serializers/EXAMPLE]]