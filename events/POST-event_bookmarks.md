<!-- --- title: POST /event_bookmarks -->

Allows the active user to create a bookmark. Each bookmark is able to reference **one** and **only** one of the following: event_user, sponsor_id, event_speaker_id, or event_session_id. If the user attempts to pass in more than one of these, the request will fail.

=
#### Authentication

The user needs to be logged in and have valid credentials to use this route.

=
#### Parameters

:event_user_id - Integer, passed in through the post data. Is derived from the 'id' field on the 'event_users' table.

:sponsor_id - Integer, passed in through the post data. Is derived from the 'id' field on the 'sponsors' table.

:event_speaker_id - Integer, passed in through the post data. Is derived from the 'id' field on the 'event_speakers' table.

:event_session_id - Integer, passed in through the post data. Is derived from the 'id' field on the 'event_sessions' table.

=
####JSON request example:
```json
http://stage-api-access.evant.com/event_bookmarks
```

=
####Post Data:
```
{ event_bookmark: { event_session_id: 9 } }
```

=
####JSON response example:

```json
{"event_bookmark"=>
  {"id"=>3,
   "event"=>{"id"=>9, "name"=>"Rustic Wooden Shoes 9"},
   "event_user"=>nil,
   "event_speaker"=>nil,
   "event_session"=>
    {"id"=>9,
     "name"=>"Small Plastic Shirt",
     "description"=>
      "Universal mobile contingency. Reactive upward-trending intranet",
     "start_date_time"=>"2014-03-14T20:25:35.000Z",
     "end_date_time"=>"2014-03-14T21:25:35.000Z",
     "track_name"=>"Function-based even-keeled software",
     "breakout_id"=>nil,
     "session_type"=>"Ergonomic Wooden Car",
     "room_name"=>"Intelligent Granite Computer",
     "is_comments_on"=>false,
     "display_rank"=>nil},
   "sponsor"=>nil}}
```

This requests provides a <strong>HTML 201</strong> on success.