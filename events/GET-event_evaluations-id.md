<!-- --- title: GET /event_evaluations/:id -->

Returns **one** event evaluations as defined by the ID passed in.

=
#### Authentication

The user needs to be logged in and have valid credentials to use this route.

=
#### Parameters

(event_evaluations) :id - Integer, passed in through the URL. Is derived from the 'id' field of the 'event_evaluations' table.

=
####API request example:
```json
http://stage-api-access.evant.com/event_evaluations/1
```

=
####JSON response example:

```json
{"event_evaluation"=>
  {"id"=>5,
   "name"=>"RSPEC Eval 1",
   "survey_link"=>"http://www.surveygizmo.com/event/3/survey_1",
   "display_rank"=>3,
   "event"=>{"id"=>3, "name"=>"Sleek Concrete Table 3"}}}
```

This requests provides a <strong>HTML 200</strong> on success.