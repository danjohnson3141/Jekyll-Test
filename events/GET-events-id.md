<!-- --- title: GET /events/:id -->

Returns the details for **one** event.

The events that are visible to the user are filtered by whether or not that event is associated with a group that the user is a member of. Being an event_user for an event trumps all group_member requirements.

=
####Authentication:

The user needs to be logged in and have valid credentials to use this route.

=
####Parameters:

(event) :id - Integer, passed in through the URL. Is derived from the 'id' field of the 'events' table.

=
####Response:

This requests provides a <strong>HTML 200</strong> on success.

=
####API request example:
```json
http://stage-api-access.evant.com/events/11787
```

=
####JSON response example:

[[include:/json/JSON_GET_events_id]]

=
####Response Data Detail:

[[include:/serializers/event]]