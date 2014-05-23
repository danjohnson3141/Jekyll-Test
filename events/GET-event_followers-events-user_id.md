<!-- --- title: GET /event_followers/events/:user_id -->

Returns a list of **all** the events followed by one user.

=
####Authentication:

The user needs to be logged in and have valid credentials to use this route.

=
####Parameters:

:user_id - Integer, passed in through the URL. Is derived from the 'user_id' field on the 'event_followers' table.

=
####Response:

This requests provides a <strong>HTML 200</strong> on success.

=
####API request example:
```json
http://stage-api-access.evant.com/event_followers/events/35005
```

=
####JSON response example:

[[include:/json/JSON_NEEDS_EXAMPLE]]

=
####Response Data Detail:

[[include:/serializers/EXAMPLE]]