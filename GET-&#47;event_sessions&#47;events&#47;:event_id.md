Returns all of the sessions for one event.

=
#### Authentication

Declare what authentications are required

Good sample text: The user needs to be logged in and have valid credentials to use this route.

=
#### Parameters

:event_id - Integer, passed in through the URL.

=
####JSON request example:
```
http://0.0.0.0:3000/ROUTE_NAME
```

=
####JSON response example:

```
{"event_sessions"=>
  [{"id"=>602,
    "name"=>"0",
    "description"=>
     "Inverse composite monitoring. Reduced optimizing focus group",
    "start_date_time"=>"2014-02-24T21:40:56.000Z",
    "end_date_time"=>"2014-02-24T22:40:56.000Z",
    "track_name"=>"User-centric transitional hardware",
    "breakout_id"=>nil,
    "session_type"=>"Practical Plastic Car",
    "room_name"=>"Practical Granite Computer",
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
     {"id"=>5103,
      "name"=>"Intelligent Wooden Pants 24",
      "event_begin_date"=>nil,
      "event_end_date"=>nil,
      "venue_name"=>"Jakubowski, Rowe and Yundt",
      "address"=>"77061 Minerva Mountains",
      "state"=>"RI",
      "postal_code"=>"98872-7464",
      "event_follower_id"=>nil,
      "country"=>nil,
      "group"=>
       {"id"=>6417,
        "name"=>"Open Group 25",
        "description"=>"Open group 25",
        "owner_user_id"=>nil,
        "group_type"=>
         {"id"=>9969, "name"=>"Factory:Open", "description"=>"Open"},
        "owner"=>nil}},
    "event_sponsor"=>
     {"id"=>788,
      "name"=>"Purdy-Schmidt",
      "description"=>
       "Et tempore est expedita harum rerum sunt porro dicta sed ratione iusto aspernatur est.",
      "logo"=>nil,
      "url"=>nil,
      "sponsor_type"=>
       {"id"=>3451,
        "name"=>"red",
        "description"=>"Persistent intermediate architecture"}},
    "post"=>
     {"id"=>1466,
      "title"=>"Synergized eco-centric database: Practical Cotton Pants",
      "body"=>
       "---\n- Debitis maiores accusamus animi rerum dolores et qui. Magni voluptates neque officia\n  illum. Moll
      "body_markdown"=>
       "---\n- Aut et magni qui sit numquam ex. Sed sed molestiae reiciendis totam dicta. Exercitationem\n  sunt d
      "excerpt"=>"Managed zero tolerance core",
      "thumbnail_teaser_photo"=>"www.example.com/post_thumbnail.jpg",
      "display_rank"=>8,
      "view_count"=>9,
      "show_likes_count"=>false,
      "like_count"=>0,
      "post_likeable"=>false,
      "view_post_likes_list"=>false,
      "post_attachments"=>[],
      "user"=>
       {"id"=>40227,
        "first_name"=>"Roselyn",
        "last_name"=>"Grady",
        "title"=>"Random User",
        "organization_name"=>"Wisozk, Stark and Nienow",
        "photo"=>
         "https://assets.evanta.com/shared/resources/Users/large/anonymous2.jpg",
        "user_role_id"=>40229}}},
   {"id"=>603,
    "name"=>"1",
    "description"=>
     "Horizontal incremental encoding. Centralized dedicated instruction set",
    "start_date_time"=>"2014-02-24T21:40:56.000Z",
    "end_date_time"=>"2014-02-24T22:40:56.000Z",
    "track_name"=>"Quality-focused local info-mediaries",
    "breakout_id"=>nil,
    "session_type"=>"Incredible Steel Gloves",
    "room_name"=>"Ergonomic Cotton Shoes",
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
     {"id"=>5103,
      "name"=>"Intelligent Wooden Pants 24",
      "event_begin_date"=>nil,
      "event_end_date"=>nil,
      "venue_name"=>"Jakubowski, Rowe and Yundt",
      "address"=>"77061 Minerva Mountains",
      "state"=>"RI",
      "postal_code"=>"98872-7464",
      "event_follower_id"=>nil,
      "country"=>nil,
      "group"=>
       {"id"=>6417,
        "name"=>"Open Group 25",
        "description"=>"Open group 25",
        "owner_user_id"=>nil,
        "group_type"=>
         {"id"=>9969, "name"=>"Factory:Open", "description"=>"Open"},
        "owner"=>nil}},
    "event_sponsor"=>
     {"id"=>789,
      "name"=>"Fahey, Bechtelar and Zemlak",
      "description"=>
       "Voluptas reiciendis ex et aspernatur ipsum blanditiis rerum perspiciatis porro.",
      "logo"=>nil,
      "url"=>nil,
      "sponsor_type"=>
       {"id"=>3453,
        "name"=>"orange",
        "description"=>"Monitored optimal emulation"}},
    "post"=>
     {"id"=>1467,
      "title"=>"Organized high-level parallelism: Fantastic Cotton Car",
      "body"=>
       "---\n- Quas ducimus nesciunt aut minima dolor tempora. Eius expedita ut. Occaecati quo\n  non. Ducimus exp
      "body_markdown"=>
       "---\n- Omnis cupiditate voluptatem reprehenderit placeat repudiandae. Cupiditate sed ipsum\n  aut pariatur
      "excerpt"=>"Reduced executive protocol",
      "thumbnail_teaser_photo"=>"www.example.com/post_thumbnail.jpg",
      "display_rank"=>0,
      "view_count"=>7,
      "show_likes_count"=>false,
      "like_count"=>0,
      "post_likeable"=>false,
      "view_post_likes_list"=>false,
      "post_attachments"=>[],
      "user"=>
       {"id"=>40233,
        "first_name"=>"Vernon",
        "last_name"=>"Cormier",
        "title"=>"Random User",
        "organization_name"=>"Leuschke, Sanford and Aufderhar",
        "photo"=>
         "https://assets.evanta.com/shared/resources/Users/large/anonymous2.jpg",
        "user_role_id"=>40235}}},
   {"id"=>601,
    "name"=>"Small Plastic Pants",
    "description"=>
     "Proactive background hardware. Ergonomic asynchronous benchmark",
    "start_date_time"=>"2014-02-24T21:40:56.000Z",
    "end_date_time"=>"2014-02-24T22:40:56.000Z",
    "track_name"=>"Proactive foreground initiative",
    "breakout_id"=>nil,
    "session_type"=>"Small Rubber Shirt",
    "room_name"=>"Incredible Rubber Chair",
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
     {"id"=>5103,
      "name"=>"Intelligent Wooden Pants 24",
      "event_begin_date"=>nil,
      "event_end_date"=>nil,
      "venue_name"=>"Jakubowski, Rowe and Yundt",
      "address"=>"77061 Minerva Mountains",
      "state"=>"RI",
      "postal_code"=>"98872-7464",
      "event_follower_id"=>nil,
      "country"=>nil,
      "group"=>
       {"id"=>6417,
        "name"=>"Open Group 25",
        "description"=>"Open group 25",
        "owner_user_id"=>nil,
        "group_type"=>
         {"id"=>9969, "name"=>"Factory:Open", "description"=>"Open"},
        "owner"=>nil}},
    "event_sponsor"=>
     {"id"=>787,
      "name"=>"Halvorson, McLaughlin and Bergstrom",
      "description"=>
       "Reiciendis recusandae rem accusamus numquam enim aliquam laudantium assumenda id in accusantium.",
      "logo"=>nil,
      "url"=>nil,
      "sponsor_type"=>
       {"id"=>3449,
        "name"=>"gold",
        "description"=>"Assimilated holistic process improvement"}},
    "post"=>
     {"id"=>1465,
      "title"=>
       "Triple-buffered assymetric throughput: Fantastic Plastic Gloves",
      "body"=>
       "---\n- Molestias accusamus et eligendi sint ut quos aut. Laborum doloribus tempora culpa\n  non quae. Nihi
      "body_markdown"=>
       "---\n- Repellendus placeat corrupti. Odit qui illum ea corrupti itaque et quia. Aut quo\n  molestiae volup
      "excerpt"=>"Optional value-added neural-net",
      "thumbnail_teaser_photo"=>"www.example.com/post_thumbnail.jpg",
      "display_rank"=>0,
      "view_count"=>7,
      "show_likes_count"=>false,
      "like_count"=>0,
      "post_likeable"=>false,
      "view_post_likes_list"=>false,
      "post_attachments"=>[],
      "user"=>
       {"id"=>40221,
        "first_name"=>"Katherine",
        "last_name"=>"Cremin",
        "title"=>"Random User",
        "organization_name"=>"Lueilwitz, Hackett and Erdman",
        "photo"=>
         "https://assets.evanta.com/shared/resources/Users/large/anonymous2.jpg",
        "user_role_id"=>40223}}}]}
```

This requests provides a <strong>HTML RESPONSE NUMBER</strong> on success.