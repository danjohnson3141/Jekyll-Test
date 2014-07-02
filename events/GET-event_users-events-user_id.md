<!-- --- title: GET /event_users/events/:user_id -->

This returns all the events associated with one user.

=
####Authentication:

The user needs to be logged in and have valid credentials to use this route.

=
####Parameters:

:user_id - Integer, passed in through the URL. Is derived from the 'id' field on the 'users' table.

=
####Response:

This requests provides a <strong>HTML 200</strong> on success.

=
####API request example:
```html
http://example.com/event_users/events/9675
```

=
####JSON response example:

[[include:/json/JSON_GET_event_users_events_user_id]]

=
####Response Data Detail:

[[include:/serializers/EXAMPLE]]