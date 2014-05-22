<!-- --- title: GET /events/upcoming -->

Returns a list of **all** upcoming events that are visible to the active user.

The events that are visible to the user are filtered by whether or not that event is associated with a group that the user is a member of. Being an event_user for an event trumps all group_member requirements.

=
####Authentication:

The user needs to be logged in and have valid credentials to use this route.

=
####Parameters:

None; default only.

=
####Response:

This requests provides a <strong>HTML 200</strong> on success.

=
####API request example:
```json
http://stage-api-access.evant.com/events/upcoming
```
=
####JSON response example:

[[include:/json/JSON_GET_events_upcoming]]

=
####Response Data Detail:

[[include:/serializers/event]]