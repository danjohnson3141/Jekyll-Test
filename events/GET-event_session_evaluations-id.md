<!-- --- title: GET /event_session_evaluations/:id -->

Returns **one** event_session_evaluation based on the ID passed in. These will be available to only the participants of specific sessions.

=
####Authentication:

The user needs to be logged in and have valid credentials to use this route.

=
####Parameters:
(event_session_evaluations) :id - Integer, passed in through the URL. Is derived from the 'id' field of the 'event_sessions_evaluations' table.



=
####API request example:
```json
http://stage-api-access.evant.com/event_session_evaluations/2
```

=
####JSON response example:

```json
{"event_session_evaluation"=>
  {"id"=>2,
   "name"=>"Survey for event: Practical Wooden Shoes 2",
   "survey_link"=>"http://www.surveygizmo.com/event/2/survey_1",
   "event"=>{"id"=>2, "name"=>"Practical Wooden Shoes 2"},
   "event_session"=>
    {"id"=>2,
     "name"=>"Ergonomic Steel Computer",
     "description"=>
      "Assimilated background open system. User-centric radical attitude",
     "start_date_time"=>"2014-03-31T17:06:36.000Z",
     "end_date_time"=>"2014-03-31T18:06:36.000Z",
     "track_name"=>"Ergonomic neutral migration",
     "breakout_group_id"=>4,
     "session_type"=>"Rustic Cotton Computer",
     "room_name"=>"Gorgeous Steel Gloves",
     "is_comments_on"=>true,
     "display_rank"=>81}}}
```

This requests provides a <strong>HTML 200</strong> on success.