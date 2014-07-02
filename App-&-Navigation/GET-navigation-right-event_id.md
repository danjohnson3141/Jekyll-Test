<!-- --- title: GET /navigation/right/:event_id -->

This returns the elements for the right navigation bar. Each of the buttons can be turned on and off by various app_setting records. 

=
####Authentication:

The user needs to be logged in and have valid credentials to use this route.

=
####Parameters:

:event_id - Integer, passed in through the URL. Derived from the 'id' field of the 'events' table.

=
####Response:

This requests provides a <strong>HTML 200</strong> on success.

=
####API request example:
```html
http://example.com/navigation/right/234
```

=
####JSON response example:

[[include:/json/JSON_GET_navigation_right_event_id]]

=
####Response Data Detail:

[[include:/serializers/EXAMPLE]]