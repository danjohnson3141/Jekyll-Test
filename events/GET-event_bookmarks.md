<!-- --- title: GET /event_bookmarks -->

This returns *all* the event_bookmarks for *one* user, regardless of type of bookmark (sessions, speaker, et al) or event.

=
####Authentication:

The user needs to be logged in and have valid credentials to use this route.

=
####Parameters:

None; default only.

=
####Response:

This requests provides a <strong>HTML 200</strong> on success.

=
####API request example:
```json
http://stage-api-access.evant.com/event_bookmarks
```

=
####JSON response example:

Returns an array of event_bookmark_short objects

[[include:/json/JSON_GET_event_bookmarks]]

=
####Response Data Detail:

[[include:/serializers/event_bookmark_short]]