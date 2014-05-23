<!-- --- title: GET /event_evaluations -->

Returns a list of **all** evaluations for **all** events that the active_user has an event_user record for.

=
####Authentication:

The user needs to be logged in and have valid credentials to use this route.

=
####Parameters:

None, default only

=
####Response:

This requests provides a <strong>HTML 200</strong> on success.

=
####API request example:
```json
http://stage-api-access.evant.com//event_evaluations
```

=
####JSON response example:

[[include:/json/JSON_GET_event_evaluations]]

=
####Response Data Detail:

[[include:/serializers/EXAMPLE]]