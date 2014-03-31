<!-- --- title: GET /event_evaluations/event/:event_id -->

Returns **all** of the event_evaluations for **one** event. The active_users needs to have an event_user record for this event in order to get the record.

=
#### Authentication

The user needs to be logged in and have valid credentials to use this route.

=
#### Parameters

:event_id - Integer, passed in through the URL. Is derived from the 'id' field of the 'events' table.

=
####JSON request example:
```json
http://0.0.0.0:3000/event_evaluations/event/5
```

=
####JSON response example:

```json
{"event_evaluations"=>
  [{"id"=>10,
    "survey_link"=>"http://www.surveygizmo.com/event/5/survey_2",
    "event_id"=>5,
    "display_rank"=>1},
   {"id"=>9,
    "survey_link"=>"http://www.surveygizmo.com/event/5/survey_1",
    "event_id"=>5,
    "display_rank"=>2},
   {"id"=>11,
    "survey_link"=>"http://www.surveygizmo.com/event/5/survey_3",
    "event_id"=>5,
    "display_rank"=>3}]}
```

This requests provides a <strong>HTML 200</strong> on success.