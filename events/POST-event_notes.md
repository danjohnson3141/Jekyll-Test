<!-- --- title: POST /event_notes -->

Allows the active user to create a note. Each note is able to reference **one** and **only** one of the following: event_user, sponsor_id, event_speaker_id, or event_session_id. If the user attempts to pass in more than one of these, the request will fail.

=
#### Authentication

The user needs to be logged in and have valid credentials to use this route.

=
#### Parameters

:body - Text, passed in through the post data. This is the plain text of the submission.

:event_user_id - Integer, passed in through the post data. Is derived from the 'id' field on the 'event_users' table.

:sponsor_id - Integer, passed in through the post data. Is derived from the 'id' field on the 'sponsors' table.

:event_speaker_id - Integer, passed in through the post data. Is derived from the 'id' field on the 'event_speakers' table.

:event_session_id - Integer, passed in through the post data. Is derived from the 'id' field on the 'event_sessions' table.

=
####API request example:
```json
http://stage-api-access.evant.com/event_notes
```

####Post Data:
```
{ event_note: { body: 'This text is the body of the note.', event_session_id: 21 }
```

=
####JSON response example:

```json
{"event_note"=>
  {"id"=>11,
   "body"=>"This text is the body of the note.",
   "event"=>{"id"=>21, "name"=>"Intelligent Concrete Computer 21"},
   "event_user"=>nil,
   "event_speaker"=>nil,
   "event_session"=>
    {"id"=>21,
     "name"=>"Fantastic Wooden Pants",
     "description"=>
      "Open-architected didactic concept. Automated local middleware",
     "start_date_time"=>"2014-03-14T20:46:27.000Z",
     "end_date_time"=>"2014-03-14T21:46:27.000Z",
     "track_name"=>"Optional bi-directional success",
     "breakout_id"=>nil,
     "session_type"=>"Intelligent Rubber Chair",
     "room_name"=>"Small Steel Pants",
     "is_comments_on"=>false,
     "display_rank"=>nil},
   "sponsor"=>nil}}
```

This requests provides a <strong>HTML 201</strong> on success.