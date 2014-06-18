<!-- --- title: GET /event_notes/event/:event_id -->

Returns **all** of the active user's event notes for **one** event.

=
####Authentication:

The user needs to be logged in and have valid credentials to use this route.

=
####Parameters:

:event_id - Integer, passed in through the URL. Is derived from the 'id' field of the 'events' table.

=
####API request example:
```html
http://example.com/event_notes/event/6038
```

=
####JSON response example:

```json
{"event_notes"=>
  [{"id"=>871,
    "body"=>
     "In voluptatem voluptatibus quisquam architecto enim ipsam ea. Asperiores quia modi numquam. Quos et necessit
    "event"=>{"id"=>6038, "name"=>"Awesome Plastic Chair 41"},
    "event_user"=>nil,
    "event_speaker"=>nil,
    "event_session"=>
     {"id"=>1947,
      "name"=>"Fantastic Granite Table",
      "description"=>
       "Compatible motivating hierarchy. Cross-platform 5th generation customer loyalty",
      "start_date_time"=>"2014-03-12T20:49:06.000Z",
      "end_date_time"=>"2014-03-12T21:49:06.000Z",
      "track_name"=>"Polarised dedicated adapter",
      "breakout_id"=>nil,
      "session_type"=>"Small Granite Shoes",
      "room_name"=>"Awesome Rubber Chair",
      "is_comments_on"=>false,
      "display_rank"=>nil},
    "sponsor"=>nil},
   {"id"=>872,
    "body"=>
     "Expedita nulla nostrum mollitia labore quod blanditiis. Tempore explicabo esse inventore. Neque occaecati cu
    "event"=>{"id"=>6038, "name"=>"Awesome Plastic Chair 41"},
    "event_user"=>nil,
    "event_speaker"=>
     {"id"=>926,
      "user_id"=>35096,
      "first_name"=>"Vincent",
      "last_name"=>"Bruen",
      "title"=>"Ergonomic Wooden Computer",
      "organization_name"=>"Hackett, Cassin and Schulist",
      "bio"=>
       "Aperiam id nesciunt. Amet voluptas placeat vero eos expedita. Inventore necessitatibus culpa explicabo et.
      "speaker_type"=>"Intelligent Granite Computer",
      "photo"=>
       "https://assets.evanta.com/shared/resources/Users/large/anonymous2.jpg",
      "event_session_id"=>1947},
    "event_session"=>nil,
    "sponsor"=>nil},
   {"id"=>873,
    "body"=>
     "Quia veniam temporibus accusamus et. Voluptate hic maiores perspiciatis. Doloremque laborum aliquid. Ut fuga
    "event"=>{"id"=>6038, "name"=>"Awesome Plastic Chair 41"},
    "event_user"=>
     {"id"=>2253,
      "user"=>
       {"id"=>35081,
        "first_name"=>"Generic",
        "last_name"=>"User",
        "title"=>"CEO of QA",
        "organization_name"=>"Evanta",
        "photo"=>
         "https://assets.evanta.com/shared/resources/Users/large/anonymous2.jpg",
        "user_role_id"=>34751,
        "user_connection_id"=>nil}},
    "event_speaker"=>nil,
    "event_session"=>nil,
    "sponsor"=>nil},
   {"id"=>874,
    "body"=>
     "Repellendus laborum in nisi magni doloremque corrupti. Alias unde cupiditate quis. Corrupti porro facilis ve
    "event"=>{"id"=>6038, "name"=>"Awesome Plastic Chair 41"},
    "event_user"=>nil,
    "event_speaker"=>nil,
    "event_session"=>nil,
    "sponsor"=>
     {"id"=>3234,
      "name"=>"Anderson, Daugherty and Koch 41",
      "description"=>
       "Qui voluptate excepturi nesciunt et placeat voluptatibus necessitatibus sint repellat corporis enim ducimu
      "logo"=>"www.example.com/sponsor_logo.jpg",
      "url"=>"goyettestanton.org",
      "event_note_id"=>874,
      "event_bookmark_id"=>nil,
      "sponsor_type"=>
       {"id"=>3234,
        "name"=>"indigo",
        "description"=>"Visionary value-added firmware",
        "display_rank"=>77},
      "banner_ads"=>[]}}]}
```

This requests provides a <strong>HTML 200</strong> on success.