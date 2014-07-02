<!-- --- title: GET /event_council_members/event/:event_id -->

Returns a list of **all** event_council_members for **one** event.

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
http://example.com/event_council_members/event/4
```

=
####JSON response example:

consists of an array of event_council_member objects

[[include:/json/JSON_GET_event_council_members_event_event_id]]

=
####Response Data Detail:

[[include:/serializers/event_council_member]]