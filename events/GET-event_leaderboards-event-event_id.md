<!-- --- title: GET /event_leaderboards/event/:event_id -->

Returns the current leaderboard rules for **one** event

=
####Authentication:

The user needs to be logged in and have valid credentials to use this route.

=
####Parameters:

:event_id - Integer, passed in throug the post data. Is derived from the 'id' field on the 'events' table.

=
####Response:

This requests provides a <strong>HTML 200</strong> on success.

=
####API request example:
```html
http://example.com/event_leaderboards/event/4
```

=
####JSON response example:

[[include:/json/JSON_GET_event_leaderboards_event_event_id]]

=
####Response Data Detail:

[[include:/serializers/EXAMPLE]]