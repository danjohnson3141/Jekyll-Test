<!-- --- title: GET /event_evaluations -->

Returns a list of **all** evaluations for **all** events that the active_user has an event_user record for.

=
#### Authentication

The user needs to be logged in and have valid credentials to use this route.

=
#### Parameters

none, default only

=
####JSON request example:
```json
http://stage-api-access.evant.com//event_evaluations
```

=
####JSON response example:

```json
{"event_evaluations"=>
  [{"id"=>14,
    "survey_link"=>"http://www.surveygizmo.com/event/7/survey_2",
    "event_id"=>7,
    "display_rank"=>1},
   {"id"=>13,
    "survey_link"=>"http://www.surveygizmo.com/event/7/survey_1",
    "event_id"=>7,
    "display_rank"=>2},
   {"id"=>15,
    "survey_link"=>"http://www.surveygizmo.com/event/7/survey_3",
    "event_id"=>7,
    "display_rank"=>3},
   {"id"=>16,
    "survey_link"=>"http://www.surveygizmo.com/event/7/survey_3",
    "event_id"=>8,
    "display_rank"=>3}]}
```

This requests provides a <strong>HTML 200</strong> on success.