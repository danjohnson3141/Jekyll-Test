<!-- --- title: DELETE /event_user_schedules/:id -->

Removes the event user schedule record from the database. 

=
####Authentication:

The user needs to be logged in and have valid credentials to use this route.

=
####Parameters:

(event_user_schedules) :id - Integer, passed in through the URL. Is derived from the 'id' field of the 'event_user_schedules' table.

=
####API request example:
```json
http://stage-api-access.evant.com/event_user_schedules/234
```

=
####JSON response example:

[[include:/json/JSON_NO_RESPONSE]]

This requests provides a <strong>HTML 204</strong> on success.