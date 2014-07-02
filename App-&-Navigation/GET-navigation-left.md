<!-- --- title: GET /navigation/left -->

This is a route to help populate the left navigation element in the app (e.g. clicking on the bug).

The 'user_today_events' field of the json only returns events that the user is registered for or is attending. This comes off of the 'event_registration_status_id' field of the 'event_users' table.

=
####Authentication:

The user needs to be logged in and have valid credentials to use this route.

####Parameters:

This route has no parameters and returns its content based on the users's internal settings.

=
####Response:

This requests provides a <strong>HTML 200</strong> on success.

=
####API request example:
```html
http://example.com/navigation/left
```

=
####JSON response example:

[[include:/json/JSON_GET_navigation_left]]

=
####Response Data Detail:

[[include:/serializers/EXAMPLE]]