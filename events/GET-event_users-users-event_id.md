<!-- --- title: GET /event_users/users/:event_id -->

This returns all the event users for one event.

=
####Authentication:

The user needs to be logged in and have valid credentials to use this route.

=
####Parameters:

:event_id - Integer, passed in through the URL. Is derived from the 'event_id' field on the 'event_users' table.

=
####Response:

This requests provides a <strong>HTML 200</strong> on success.

=
####API request example:
```html
http://example.com/event_users/users/10579
```

=
####JSON response example:

Returns an array of event_user_tiny objects

[[include:/json/JSON_GET_event_users_users_event_id]]

=
####Response Data Detail:

[[include:/serializers/event_user_tiny]]