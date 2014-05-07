<!-- --- title: POST /event_user_schedules -->

This is how the active user creates event_user_schedule records. These records are used to create the user's "My Schedule".

=
#### Authentication

The user needs to be logged in and have valid credentials to use this route.

=
#### Parameters

:event_session_id - Integer, passed in through the post data. Is derived from the 'id' field on the 'event_sessions' table.

=
####JSON request example:
```json
http://stage-api-access.evant.com/event_user_schedules
```

=
####Post Data:
```json
{ event_user_schedule: { event_session_id: 1527 } }
```

=
####JSON response example:

```json
{"event_user_schedule"=>
  {"id"=>477,
   "event_session"=>
    {"id"=>1527,
     "name"=>"Practical Wooden Car",
     "description"=>
      "Seamless global benchmark. Assimilated optimizing neural-net",
     "start_date_time"=>"2014-03-18T18:10:15.000Z",
     "end_date_time"=>"2014-03-18T19:10:15.000Z",
     "track_name"=>"Organic optimal methodology",
     "breakout_id"=>nil,
     "session_type"=>"Practical Concrete Pants",
     "room_name"=>"Ergonomic Wooden Gloves",
     "is_comments_on"=>false,
     "display_rank"=>nil},
   "event_user"=>
    {"id"=>1842,
     "user"=>
      {"id"=>23778,
       "first_name"=>"Generic",
       "last_name"=>"User",
       "title"=>"CEO of QA",
       "organization_name"=>"Evanta",
       "photo"=>
        "https://assets.evanta.com/shared/resources/Users/large/anonymous2.jpg",
       "user_role_id"=>28021,
       "user_connection_id"=>nil}}}}
```

This requests provides a <strong>HTML 201</strong> on success.