<!-- --- title: GET /event_evaluations/event/:event_id -->

Returns **all** of the event_evaluations for **one** event. The active_users needs to have an event_user record for this event in order to get the record.

=
####Authentication:

The user needs to be logged in and have valid credentials to use this route.

=
####Parameters:

:event_id - Integer, passed in through the URL. Is derived from the 'id' field of the 'events' table.

=
####Response:

This requests provides a <strong>HTML 200</strong> on success.

=
####API request example:
```html
http://stage-api-access.evant.com/event_evaluations/event/5
```

=
####JSON response example:

Returns an array of event_evaluation objects

[[include:/json/JSON_GET_event_evaluations_event_event_id]]

=
####Response Data Detail:

[[include:/serializers/event_evaluation]]