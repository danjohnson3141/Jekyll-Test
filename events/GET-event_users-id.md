<!-- --- title: GET /event_users/:id -->

Returns informtion on **one** event_user

=
####Authentication:

The user needs to be logged in and have valid credentials to use this route.

=
####Parameters:

:id - Integer, passed in through the URL. Is derived from the 'id' field of the 'event_users' table.

=
####Response:

This requests provides a <strong>HTML 200</strong> on success.

=
####API request example:
```html
http://example.com/event_users/2
```

=
####JSON response example:

[[include:GET-event_users-id]]

=
####Response Data Detail:

[[include:/serializers/EXAMPLE]]