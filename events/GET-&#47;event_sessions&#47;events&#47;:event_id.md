<!-- --- title: GET /event_sessions/events/:event_id -->

Returns all of the sessions for one event.

=
#### Authentication

The user needs to be logged in and have valid credentials to use this route.

=
#### Parameters

:event_id - Integer, passed in through the URL. Is derived from the 'event_id' field on the 'event_sessions' table.

=
####JSON request example:
```
http://0.0.0.0:3000/event_sessions/events/5363
```

=
####JSON response example:

```json
{"event_sessions"=>
  [{"id"=>617,
    "name"=>"0",
    "description"=>
     "Monitored composite paradigm. De-engineered modular installation",
    "start_date_time"=>"2014-02-24T21:46:10.000Z",
    "end_date_time"=>"2014-02-24T22:46:10.000Z",
    "track_name"=>"Customer-focused maximized utilisation",
    "breakout_id"=>nil,
    "session_type"=>"Awesome Concrete Computer",
    "room_name"=>"Rustic Wooden Pants",
    "is_comments_on"=>false,
    "event_speakers"=>[],
    "breakout_session"=>nil,
    "comment_count"=>0,
    "can_add_event_session_to_schedule"=>false,
    "can_add_notes_to_event_sessions"=>false,
    "can_bookmark_event_sessions"=>false,
    "show_event_session_evaluations"=>false,
    "event_session_evaluations"=>[],
    "secret_group_member"=>nil,
    "session_post_likeable"=>false,
    "session_commentable"=>false,
    "event"=>
     {"id"=>5363,
      "name"=>"Awesome Rubber Pants 23",
      "event_begin_date"=>nil,
      "event_end_date"=>nil,
      "venue_name"=>"Stracke and Sons",
      "address"=>"1210 Carol Orchard",
      "state"=>"ND",
      "postal_code"=>"60050",
      "event_follower_id"=>nil,
      "country"=>nil,
      "group"=>
       {"id"=>6683,
        "name"=>"Open Group 42",
        "description"=>"Open group 42",
        "owner_user_id"=>nil,
        "group_type"=>
         {"id"=>10465, "name"=>"Factory:Open", "description"=>"Open"},
        "owner"=>nil}},
    "event_sponsor"=>
     {"id"=>815,
      "name"=>"Brekke-Krajcik",
      "description"=>
       "Fugit et minus quo nam eaque accusamus at consequuntur quae ea veniam quos voluptas voluptas.",
      "logo"=>nil,
      "url"=>nil,
      "sponsor_type"=>
       {"id"=>3583,
        "name"=>"lavender",
        "description"=>"Polarised content-based success"}},
    "post"=>
     {"id"=>1508,
      "title"=>
       "Persistent zero tolerance open architecture: Intelligent Plastic Table",
      "body"=>
       "---\n- Deserunt dolores quo at modi assumenda. Totam odit temporibus dolorem similique\n  deleniti. Iusto 
      "body_markdown"=>
       "---\n- Dolorum ut deleniti. Modi asperiores est dolor sit natus eius. Aut sunt veritatis.\n- Maxime invent
      "excerpt"=>"Customizable leading edge intranet",
      "thumbnail_teaser_photo"=>"www.example.com/post_thumbnail.jpg",
      "display_rank"=>0,
      "view_count"=>0,
      "show_likes_count"=>false,
      "like_count"=>0,
      "post_likeable"=>false,
      "view_post_likes_list"=>false,
      "post_attachments"=>[],
      "user"=>
       {"id"=>41871,
        "first_name"=>"Carter",
        "last_name"=>"Volkman",
        "title"=>"Random User",
        "organization_name"=>"Aufderhar and Sons",
        "photo"=>
         "https://assets.evanta.com/shared/resources/Users/large/anonymous2.jpg",
        "user_role_id"=>41873}}},
   {"id"=>616,
    "name"=>"Awesome Steel Hat",
    "description"=>
     "Open-source context-sensitive Graphical User Interface. Proactive tangible synergy",
    "start_date_time"=>"2014-02-24T21:46:10.000Z",
    "end_date_time"=>"2014-02-24T22:46:10.000Z",
    "track_name"=>"Multi-layered even-keeled functionalities",
    "breakout_id"=>nil,
    "session_type"=>"Practical Rubber Computer",
    "room_name"=>"Awesome Steel Hat",
    "is_comments_on"=>false,
    "event_speakers"=>[],
    "breakout_session"=>nil,
    "comment_count"=>0,
    "can_add_event_session_to_schedule"=>false,
    "can_add_notes_to_event_sessions"=>false,
    "can_bookmark_event_sessions"=>false,
    "show_event_session_evaluations"=>false,
    "event_session_evaluations"=>[],
    "secret_group_member"=>nil,
    "session_post_likeable"=>false,
    "session_commentable"=>false,
    "event"=>
     {"id"=>5363,
      "name"=>"Awesome Rubber Pants 23",
      "event_begin_date"=>nil,
      "event_end_date"=>nil,
      "venue_name"=>"Stracke and Sons",
      "address"=>"1210 Carol Orchard",
      "state"=>"ND",
      "postal_code"=>"60050",
      "event_follower_id"=>nil,
      "country"=>nil,
      "group"=>
       {"id"=>6683,
        "name"=>"Open Group 42",
        "description"=>"Open group 42",
        "owner_user_id"=>nil,
        "group_type"=>
         {"id"=>10465, "name"=>"Factory:Open", "description"=>"Open"},
        "owner"=>nil}},
    "event_sponsor"=>
     {"id"=>814,
      "name"=>"Yundt, Schmidt and Senger",
      "description"=>
       "Veniam est et est dolores illum culpa cum exercitationem sed eum eius eos.",
      "logo"=>nil,
      "url"=>nil,
      "sponsor_type"=>
       {"id"=>3581,
        "name"=>"grey",
        "description"=>"Streamlined bifurcated orchestration"}},
    "post"=>
     {"id"=>1507,
      "title"=>"Expanded optimal encryption: Sleek Steel Gloves",
      "body"=>
       "---\n- Praesentium enim ipsam illum minus. Ea illo ut ea earum et. Nam illo aliquam ut.\n  Inventore molli
      "body_markdown"=>
       "---\n- Ut velit soluta. Voluptates enim eos consequatur sit vel pariatur. Voluptatem sit\n  iure quis. Min
      "excerpt"=>"Customer-focused national database",
      "thumbnail_teaser_photo"=>"www.example.com/post_thumbnail.jpg",
      "display_rank"=>4,
      "view_count"=>2,
      "show_likes_count"=>false,
      "like_count"=>0,
      "post_likeable"=>false,
      "view_post_likes_list"=>false,
      "post_attachments"=>[],
      "user"=>
       {"id"=>41865,
        "first_name"=>"Howell",
        "last_name"=>"Bogan",
        "title"=>"Random User",
        "organization_name"=>"Paucek and Sons",
        "photo"=>
         "https://assets.evanta.com/shared/resources/Users/large/anonymous2.jpg",
        "user_role_id"=>41867}}}]}
```

This requests provides a <strong>HTML 200</strong> on success.