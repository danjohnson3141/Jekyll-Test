<!-- --- title: GET /events/all -->

Returns **all** the events for the active user for which they have _either_ an event_follower or event_user record. 

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
```html
http://stage-api-access.evant.com/events/all
```

=
####JSON response example:

[[include:/json/JSON_GET_events_all]]

=
####Response Data Detail:

[[include:/serializers/event]]