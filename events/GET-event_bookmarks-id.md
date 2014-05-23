<!-- --- title: GET /event_bookmarks/:id -->

Returns **one** event bookmark based on the id passed in.

=
####Authentication:

The user needs to be logged in and have valid credentials to use this route.

=
####Parameters:

(event_bookmarks) :id - Integer, passed in the URL. Is derived from the 'id' field on the the 'event_bookmarks' table.

=
####Response:

This requests provides a <strong>HTML 200</strong> on success.

=
####API request example:
```html
http://stage-api-access.evant.com/event_bookmarks/81
```

=
####JSON response example:

[[include:/json/JSON_GET_event_bookmarks_id]]

=
####Response Data Detail:

[[include:/serializers/event_bookmark_short]]