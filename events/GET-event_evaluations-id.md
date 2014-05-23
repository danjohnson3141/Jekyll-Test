<!-- --- title: GET /event_evaluations/:id -->

Returns **one** event evaluations as defined by the ID passed in.

=
####Authentication:

The user needs to be logged in and have valid credentials to use this route.

=
####Parameters:

(event_evaluations) :id - Integer, passed in through the URL. Is derived from the 'id' field of the 'event_evaluations' table.

=
####Response:

This requests provides a <strong>HTML 200</strong> on success.

=
####API request example:
```html
http://stage-api-access.evant.com/event_evaluations/1
```

=
####JSON response example:

[[include:/json/JSON_GET_event_evaluations_id]]

=
####Response Data Detail:

[[include:/serializers/event_evaluation]]