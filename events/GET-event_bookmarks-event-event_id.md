<!-- --- title: GET /event_bookmarks/event/:event_id -->

This route returns **all** of the bookmarks that the active user has for **one** event.

=
####Authentication:

The user needs to be logged in and have valid credentials to use this route.

=
####Parameters:

:event_id - Integer, passed in through the URL. Is derived from the 'id' field of the 'events' table.

=
####API request example:
```json
http://stage-api-access.evant.com/event_bookmarks/event/2904
```

=
####JSON response example:

```json
{"event_bookmarks"=>
  [{"id"=>451,
    "event"=>{"id"=>2904, "name"=>"Fantastic Wooden Shoes 383"},
    "event_user"=>
     {"id"=>1008,
      "user"=>
       {"id"=>18415,
        "first_name"=>"Generic",
        "last_name"=>"User",
        "title"=>"CEO of QA",
        "organization_name"=>"Evanta",
        "photo"=>
         "https://assets.evanta.com/shared/resources/Users/large/anonymous2.jpg",
        "user_role_id"=>18217,
        "user_connection_id"=>nil}},
    "event_speaker"=>nil,
    "event_session"=>nil,
    "sponsor"=>nil},
   {"id"=>452,
    "event"=>{"id"=>2904, "name"=>"Fantastic Wooden Shoes 383"},
    "event_user"=>nil,
    "event_speaker"=>
     {"id"=>331,
      "user_id"=>18430,
      "first_name"=>"Abraham",
      "last_name"=>"Schowalter",
      "title"=>"Rustic Concrete Car",
      "organization_name"=>"Johnson, Haley and Greenfelder",
      "bio"=>
       "Aut et accusantium. Eligendi error consequatur eos numquam dolorum delectus doloremque. Nesciunt quod quia
      "speaker_type"=>"Incredible Plastic Chair",
      "photo"=>
       "https://assets.evanta.com/shared/resources/Users/large/anonymous2.jpg",
      "event_session_id"=>923},
    "event_session"=>nil,
    "sponsor"=>nil},
   {"id"=>453,
    "event"=>{"id"=>2904, "name"=>"Fantastic Wooden Shoes 383"},
    "event_user"=>nil,
    "event_speaker"=>nil,
    "event_session"=>
     {"id"=>923,
      "name"=>"Gorgeous Wooden Car",
      "description"=>
       "Organic contextually-based strategy. Integrated regional functionalities",
      "start_date_time"=>"2014-03-12T20:15:37.000Z",
      "end_date_time"=>"2014-03-12T21:15:37.000Z",
      "track_name"=>"Virtual intermediate artificial intelligence",
      "breakout_id"=>nil,
      "session_type"=>"Rustic Steel Car",
      "room_name"=>"Sleek Plastic Hat",
      "is_comments_on"=>false,
      "display_rank"=>nil},
    "sponsor"=>nil},
   {"id"=>454,
    "event"=>{"id"=>2904, "name"=>"Fantastic Wooden Shoes 383"},
    "event_user"=>nil,
    "event_speaker"=>nil,
    "event_session"=>nil,
    "sponsor"=>
     {"id"=>1448,
      "name"=>"Effertz, Jakubowski and Schneider 244",
      "description"=>
       "Voluptatum ut blanditiis quia ab praesentium illo distinctio sit incidunt quasi eaque sed et officiis.",
      "logo"=>"www.example.com/sponsor_logo.jpg",
      "url"=>"eichmanntowne.com",
      "event_note_id"=>nil,
      "event_bookmark_id"=>454,
      "sponsor_type"=>
       {"id"=>1448,
        "name"=>"sky blue",
        "description"=>"Distributed multi-tasking interface",
        "display_rank"=>14},
      "banner_ads"=>[]}}]}
```

This requests provides a <strong>HTML 200</strong> on success.