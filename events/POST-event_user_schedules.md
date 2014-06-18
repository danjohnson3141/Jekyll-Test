<!-- --- title: POST /event_user_schedules -->

This is how the active user creates event_user_schedule records. These records are used to create the user's "My Schedule".

=
####Authentication:

The user needs to be logged in and have valid credentials to use this route.

=
####Parameters:

:event_session_id - Integer, passed in through the post data. Is derived from the 'id' field on the 'event_sessions' table.

=
####Response:

This requests provides a <strong>HTML 201</strong> on success.

=
####API request example:
```html
http://example.com/event_user_schedules
```

=
####Post data example::
```json
{ event_user_schedule: 
	{ event_session_id: 1527 } }
``` 
 
=
###Post data detail:

[[include:/post_data/post_event_user_schedules]]

=
####JSON response example:

[[include:/json/JSON_POST_event_user_schedules]]

=
####Response Data Detail:

[[include:/serializers/event_user_schedule_short]]