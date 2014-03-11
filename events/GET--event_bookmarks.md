<!-- --- title: GET /event_bookmarks -->

This returns *all* the event_bookmarks for *one* user, regardless of type of bookmark (sessions, speaker, et al) or event.

=
#### Authentication

The user needs to be logged in and have valid credentials to use this route.

=
#### Parameters

None; default only.

=
####JSON request example:
```
http://0.0.0.0:3000/event_bookmarks
```

=
####JSON response example:
```json
{"event_bookmarks"=>
  [{"id"=>1089,
    "event"=>{"id"=>6928, "name"=>"Gorgeous Concrete Chair 1"},
    "event_user"=>
     {"id"=>2583,
      "user"=>
       {"id"=>38103,
        "first_name"=>"Generic",
        "last_name"=>"User",
        "title"=>"CEO of QA",
        "organization_name"=>"Evanta",
        "photo"=>
         "https://assets.evanta.com/shared/resources/Users/large/anonymous2.jpg",
        "user_role_id"=>37707,
        "user_connection_id"=>nil}},
    "event_speaker"=>nil,
    "event_session"=>nil,
    "sponsor"=>nil},
   {"id"=>1090,
    "event"=>{"id"=>6929, "name"=>"Awesome Steel Table 2"},
    "event_user"=>
     {"id"=>2584,
      "user"=>
       {"id"=>38103,
        "first_name"=>"Generic",
        "last_name"=>"User",
        "title"=>"CEO of QA",
        "organization_name"=>"Evanta",
        "photo"=>
         "https://assets.evanta.com/shared/resources/Users/large/anonymous2.jpg",
        "user_role_id"=>37707,
        "user_connection_id"=>nil}},
    "event_speaker"=>nil,
    "event_session"=>nil,
    "sponsor"=>nil}]}
```json

This requests provides a <strong>HTML 200</strong> on success.