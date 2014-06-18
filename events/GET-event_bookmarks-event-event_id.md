<!-- --- title: GET /event_bookmarks/event/:event_id -->

This route returns **all** of the bookmarks that the active user has for **one** event.

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
http://example.com/event_bookmarks/event/2904
```

=
####JSON response example:

Returns an array of event_bookmark_short objects

[[include:/json/JSON_GET_event_bookmarks_event_event_id]]

=
####Response Data Detail:


[[include:/serializers/event_bookmark_short]]