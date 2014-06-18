<!-- --- title: GET /app_labels/event/:event_id -->

Returns a list of labels specific to an event. 

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
http://example.com/app_labels/event/4
```

=
####JSON response example:

[[include:/json/JSON_GET_app_labels_event_event_id]]

=
####Response Data Detail:

[[include:/serializers/app_label]]