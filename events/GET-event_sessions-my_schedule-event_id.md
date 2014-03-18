<!-- --- title: GET /event_sessions/my_schedule/:event_id -->

This returns **all** the event_user_schedule records associated with the active user for **one** event.

=
#### Authentication

The user needs to be logged in and have valid credentials to use this route.

=
#### Parameters

:event_id - Integer, passed in through the URL. Is derived from the 'id' field of the 'events' table.

=
####JSON request example:
```json
http://0.0.0.0:3000/event_sessions/my_schedule/6126
```

=
####JSON response example:

```json
{"event_sessions"=>
  [{"id"=>2005,
    "name"=>"C",
    "description"=>
     "Reduced bottom-line system engine. Multi-tiered mission-critical algorithm",
    "start_date_time"=>"2014-03-11T14:44:45.000Z",
    "end_date_time"=>"2014-03-12T22:03:36.000Z",
    "track_name"=>"Streamlined user-facing extranet",
    "breakout_id"=>nil,
    "session_type"=>"Awesome Granite Pants",
    "room_name"=>"Small Steel Chair",
    "is_comments_on"=>false,
    "breakout_session"=>nil,
    "comment_count"=>1,
    "show_my_schedule"=>true,
    "show_event_notes"=>true,
    "show_bookmarks"=>true,
    "show_event_session_evaluations"=>true,
    "event_session_evaluations"=>[],
    "secret_group_member"=>nil,
    "show_post_likes"=>true,
    "session_comments"=>true,
    "event_note_id"=>906,
    "event_bookmark_id"=>869,
    "event_schedule_id"=>638,
    "display_rank"=>1,
    "event"=>{"id"=>6126, "name"=>"Intelligent Granite Pants 49"},
    "sponsor"=>
     {"id"=>3310,
      "name"=>"Funk LLC 39",
      "description"=>
       "Quo quia blanditiis ut eaque quia neque delectus sed quaerat nihil rem.",
      "logo"=>"www.example.com/sponsor_logo.jpg",
      "url"=>"kautzer.info",
      "event_note_id"=>nil,
      "event_bookmark_id"=>nil,
      "sponsor_type"=>
       {"id"=>3310,
        "name"=>"yellow",
        "description"=>"Cloned background function",
        "display_rank"=>90},
      "banner_ads"=>[]},
    "post"=>
     {"id"=>3238,
      "title"=>"Synergistic composite toolset: Fantastic Granite Chair",
      "excerpt"=>"Focused motivating website",
      "thumbnail_teaser_photo"=>"www.example.com/post_thumbnail.jpg",
      "view_count"=>7,
      "show_likes_count"=>true,
      "like_count"=>0,
      "comment_count"=>0,
      "post_like_id"=>nil,
      "post_likes"=>true,
      "show_post_likes_list"=>true,
      "post_attachments"=>[],
      "authors"=>[nil],
      "ago"=>"0m",
      "group"=>nil,
      "event"=>{"id"=>6129, "name"=>"Small Rubber Shoes 52"}},
    "event_speakers"=>[]},
   {"id"=>2003,
    "name"=>"B",
    "description"=>
     "Customizable client-server software. Diverse intermediate complexity",
    "start_date_time"=>"2014-03-11T15:44:45.000Z",
    "end_date_time"=>"2014-03-12T22:03:36.000Z",
    "track_name"=>"Advanced national software",
    "breakout_id"=>nil,
    "session_type"=>"Awesome Granite Computer",
    "room_name"=>"Incredible Wooden Shoes",
    "is_comments_on"=>false,
    "breakout_session"=>nil,
    "comment_count"=>0,
    "show_my_schedule"=>true,
    "show_event_notes"=>true,
    "show_bookmarks"=>true,
    "show_event_session_evaluations"=>true,
    "event_session_evaluations"=>[],
    "secret_group_member"=>nil,
    "show_post_likes"=>true,
    "session_comments"=>true,
    "event_note_id"=>nil,
    "event_bookmark_id"=>868,
    "event_schedule_id"=>637,
    "display_rank"=>1,
    "event"=>{"id"=>6126, "name"=>"Intelligent Granite Pants 49"},
    "sponsor"=>
     {"id"=>3308,
      "name"=>"Greenfelder, Rutherford and Schoen 37",
      "description"=>
       "Sint eligendi explicabo modi officia rerum culpa doloremque iusto commodi amet qui voluptate voluptas.",
      "logo"=>"www.example.com/sponsor_logo.jpg",
      "url"=>"hilllhamill.name",
      "event_note_id"=>nil,
      "event_bookmark_id"=>nil,
      "sponsor_type"=>
       {"id"=>3308,
        "name"=>"ivory",
        "description"=>"Ergonomic optimizing concept",
        "display_rank"=>90},
      "banner_ads"=>[]},
    "post"=>
     {"id"=>3236,
      "title"=>"Integrated multi-state collaboration: Small Wooden Chair",
      "excerpt"=>"Organized bifurcated knowledge base",
      "thumbnail_teaser_photo"=>"www.example.com/post_thumbnail.jpg",
      "view_count"=>8,
      "show_likes_count"=>true,
      "like_count"=>0,
      "comment_count"=>0,
      "post_like_id"=>nil,
      "post_likes"=>true,
      "show_post_likes_list"=>true,
      "post_attachments"=>[],
      "authors"=>[nil],
      "ago"=>"0m",
      "group"=>nil,
      "event"=>{"id"=>6127, "name"=>"Rustic Cotton Shirt 50"}},
    "event_speakers"=>[]}]}
```

This requests provides a <strong>HTML 200</strong> on success.