<!-- --- title: GET /event_speakers/event_session/:event_session_id -->

Returns all of the speakers for one event_session.

=
#### Authentication

Declare what authentications are required
Good sample text: The user needs to be logged in and have valid credentials to use this route.

=
#### Parameters

:event_session_id - Integer, passed in through the URL. Is derived from the 'id' field

=
####JSON request example:
```json
http://0.0.0.0:3000/event_speakers/event_session/664
```

=
####JSON response example:

```json
{"event_speakers"=>
  [{"id"=>108,
    "first_name"=>"Loren",
    "last_name"=>"Schroeder",
    "title"=>"Incredible Wooden Computer",
    "organization_name"=>"Ankunding, McKenzie and Marquardt",
    "bio"=>
     "Vel amet ab vero enim. Voluptatem eos quia aut. Adipisci ut similique. Atque ea libero vero velit molestiae.
    "speaker_type"=>"Intelligent Wooden Pants",
    "moderator"=>false,
    "photo"=>
     "https://assets.evanta.com/shared/resources/Users/large/anonymous2.jpg",
    "user"=>
     {"id"=>16891,
      "email"=>"joseph@hyatt.org",
      "alt_email"=>"aniya@hotmail.com",
      "first_name"=>"Darion",
      "last_name"=>"Cassin",
      "title"=>"Random User",
      "organization_name"=>"Padberg-Lemke",
      "bio"=>"Et dicta sed ducimus ratione soluta minus qui et ea autem.",
      "photo"=>
       "https://assets.evanta.com/shared/resources/Users/large/anonymous2.jpg",
      "user_role_id"=>16847,
      "user_connection_id"=>nil},
    "event_session"=>
     {"id"=>664,
      "name"=>"Rustic Wooden Table",
      "description"=>
       "Intuitive cohesive solution. Face to face zero tolerance core",
      "start_date_time"=>"2014-02-26T22:07:13.000Z",
      "end_date_time"=>"2014-02-26T23:07:13.000Z",
      "track_name"=>"Multi-channelled tangible focus group",
      "breakout_id"=>nil,
      "session_type"=>"Ergonomic Rubber Pants",
      "room_name"=>"Incredible Steel Computer",
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
      "event"=>
       {"id"=>2220,
        "name"=>"Rustic Plastic Pants 99",
        "begin_date"=>"2014-03-08",
        "end_date"=>"2014-03-09",
        "venue_name"=>"Price, Klocko and Robel",
        "address"=>"921 Balistreri Terrace",
        "state"=>"NC",
        "postal_code"=>"30016",
        "event_follower_id"=>nil,
        "country"=>{"name"=>"Iraq", "abbreviation"=>"0n0"},
        "group"=>
         {"id"=>4053,
          "name"=>"Open Group 144",
          "description"=>"Open group 144",
          "owner_user_id"=>16881,
          "group_type"=>
           {"id"=>5466, "name"=>"Factory:Open", "description"=>"Open"},
          "owner"=>
           {"id"=>16881,
            "first_name"=>"Pauline",
            "last_name"=>"Gutkowski",
            "title"=>"Creator Of All 1",
            "organization_name"=>"Hintz, Wolff and Cummerata",
            "photo"=>
             "https://assets.evanta.com/shared/resources/Users/large/anonymous2.jpg",
            "user_role_id"=>16837,
            "user_connection_id"=>nil}}},
      "event_sponsor"=>
       {"id"=>736,
        "name"=>"Skiles-Wehner",
        "description"=>
         "Illo deleniti dolores similique nam nisi et earum atque aut.",
        "logo"=>"www.example.com/logo.bmp",
        "url"=>"www.example.com",
        "sponsor_type"=>
         {"id"=>3994,
          "name"=>"ivory",
          "description"=>"Ameliorated human-resource success"}},
      "post"=>
       {"id"=>923,
        "title"=>"Robust 4th generation ability: Incredible Concrete Car",
        "body"=>
         "---\n- Illo praesentium alias. Ducimus occaecati iure ad accusamus fugiat hic eveniet.\n  Fuga expedita 
        "body_markdown"=>
         "---\n- Voluptatem maxime minus accusantium. Voluptates eligendi consectetur. Magnam quae\n  eum.\n- Nece
        "excerpt"=>"Reverse-engineered multi-state benchmark",
        "thumbnail_teaser_photo"=>"www.example.com/post_thumbnail.jpg",
        "display_rank"=>8,
        "view_count"=>3,
        "show_likes_count"=>true,
        "like_count"=>0,
        "post_likes"=>true,
        "show_post_likes_list"=>true,
        "post_attachments"=>[],
        "user"=>
         {"id"=>16884,
          "first_name"=>"Ursula",
          "last_name"=>"McDermott",
          "title"=>"Random User",
          "organization_name"=>"Schoen LLC",
          "photo"=>
           "https://assets.evanta.com/shared/resources/Users/large/anonymous2.jpg",
          "user_role_id"=>16840,
          "user_connection_id"=>nil}},
      "event_speakers"=>
       [{"id"=>108,
         "user_id"=>16891,
         "first_name"=>"Loren",
         "last_name"=>"Schroeder",
         "title"=>"Incredible Wooden Computer",
         "organization_name"=>"Ankunding, McKenzie and Marquardt",
         "bio"=>
          "Vel amet ab vero enim. Voluptatem eos quia aut. Adipisci ut similique. Atque ea libero vero velit moles
         "speaker_type"=>"Intelligent Wooden Pants",
         "moderator"=>false,
         "photo"=>
          "https://assets.evanta.com/shared/resources/Users/large/anonymous2.jpg"},
        {"id"=>109,
         "user_id"=>16892,
         "first_name"=>"Laisha",
         "last_name"=>"Strosin",
         "title"=>"Small Wooden Hat",
         "organization_name"=>"Turner LLC",
         "bio"=>
          "Et dolores debitis porro nesciunt error. Recusandae minima accusantium eos asperiores error rerum. Eos 
         "speaker_type"=>"Ergonomic Granite Pants",
         "moderator"=>true,
         "photo"=>
          "https://assets.evanta.com/shared/resources/Users/large/anonymous2.jpg"}]}},
   {"id"=>109,
    "first_name"=>"Laisha",
    "last_name"=>"Strosin",
    "title"=>"Small Wooden Hat",
    "organization_name"=>"Turner LLC",
    "bio"=>
     "Et dolores debitis porro nesciunt error. Recusandae minima accusantium eos asperiores error rerum. Eos persp
    "speaker_type"=>"Ergonomic Granite Pants",
    "moderator"=>true,
    "photo"=>
     "https://assets.evanta.com/shared/resources/Users/large/anonymous2.jpg",
    "user"=>
     {"id"=>16892,
      "email"=>"kayleigh.grady@hand.info",
      "alt_email"=>"brielle.greenholt@gmail.com",
      "first_name"=>"Jody",
      "last_name"=>"Kilback",
      "title"=>"Random User",
      "organization_name"=>"Kessler-Barrows",
      "bio"=>
       "Est minus non aut error optio facilis eos et saepe earum odit libero molestias.",
      "photo"=>
       "https://assets.evanta.com/shared/resources/Users/large/anonymous2.jpg",
      "user_role_id"=>16848,
      "user_connection_id"=>nil},
    "event_session"=>
     {"id"=>664,
      "name"=>"Rustic Wooden Table",
      "description"=>
       "Intuitive cohesive solution. Face to face zero tolerance core",
      "start_date_time"=>"2014-02-26T22:07:13.000Z",
      "end_date_time"=>"2014-02-26T23:07:13.000Z",
      "track_name"=>"Multi-channelled tangible focus group",
      "breakout_id"=>nil,
      "session_type"=>"Ergonomic Rubber Pants",
      "room_name"=>"Incredible Steel Computer",
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
      "event"=>
       {"id"=>2220,
        "name"=>"Rustic Plastic Pants 99",
        "begin_date"=>"2014-03-08",
        "end_date"=>"2014-03-09",
        "venue_name"=>"Price, Klocko and Robel",
        "address"=>"921 Balistreri Terrace",
        "state"=>"NC",
        "postal_code"=>"30016",
        "event_follower_id"=>nil,
        "country"=>{"name"=>"Iraq", "abbreviation"=>"0n0"},
        "group"=>
         {"id"=>4053,
          "name"=>"Open Group 144",
          "description"=>"Open group 144",
          "owner_user_id"=>16881,
          "group_type"=>
           {"id"=>5466, "name"=>"Factory:Open", "description"=>"Open"},
          "owner"=>
           {"id"=>16881,
            "first_name"=>"Pauline",
            "last_name"=>"Gutkowski",
            "title"=>"Creator Of All 1",
            "organization_name"=>"Hintz, Wolff and Cummerata",
            "photo"=>
             "https://assets.evanta.com/shared/resources/Users/large/anonymous2.jpg",
            "user_role_id"=>16837,
            "user_connection_id"=>nil}}},
      "event_sponsor"=>
       {"id"=>736,
        "name"=>"Skiles-Wehner",
        "description"=>
         "Illo deleniti dolores similique nam nisi et earum atque aut.",
        "logo"=>"www.example.com/logo.bmp",
        "url"=>"www.example.com",
        "sponsor_type"=>
         {"id"=>3994,
          "name"=>"ivory",
          "description"=>"Ameliorated human-resource success"}},
      "post"=>
       {"id"=>923,
        "title"=>"Robust 4th generation ability: Incredible Concrete Car",
        "body"=>
         "---\n- Illo praesentium alias. Ducimus occaecati iure ad accusamus fugiat hic eveniet.\n  Fuga expedita 
        "body_markdown"=>
         "---\n- Voluptatem maxime minus accusantium. Voluptates eligendi consectetur. Magnam quae\n  eum.\n- Nece
        "excerpt"=>"Reverse-engineered multi-state benchmark",
        "thumbnail_teaser_photo"=>"www.example.com/post_thumbnail.jpg",
        "display_rank"=>8,
        "view_count"=>3,
        "show_likes_count"=>true,
        "like_count"=>0,
        "post_likes"=>true,
        "show_post_likes_list"=>true,
        "post_attachments"=>[],
        "user"=>
         {"id"=>16884,
          "first_name"=>"Ursula",
          "last_name"=>"McDermott",
          "title"=>"Random User",
          "organization_name"=>"Schoen LLC",
          "photo"=>
           "https://assets.evanta.com/shared/resources/Users/large/anonymous2.jpg",
          "user_role_id"=>16840,
          "user_connection_id"=>nil}},
      "event_speakers"=>
       [{"id"=>108,
         "user_id"=>16891,
         "first_name"=>"Loren",
         "last_name"=>"Schroeder",
         "title"=>"Incredible Wooden Computer",
         "organization_name"=>"Ankunding, McKenzie and Marquardt",
         "bio"=>
          "Vel amet ab vero enim. Voluptatem eos quia aut. Adipisci ut similique. Atque ea libero vero velit moles
         "speaker_type"=>"Intelligent Wooden Pants",
         "moderator"=>false,
         "photo"=>
          "https://assets.evanta.com/shared/resources/Users/large/anonymous2.jpg"},
        {"id"=>109,
         "user_id"=>16892,
         "first_name"=>"Laisha",
         "last_name"=>"Strosin",
         "title"=>"Small Wooden Hat",
         "organization_name"=>"Turner LLC",
         "bio"=>
          "Et dolores debitis porro nesciunt error. Recusandae minima accusantium eos asperiores error rerum. Eos 
         "speaker_type"=>"Ergonomic Granite Pants",
         "moderator"=>true,
         "photo"=>
          "https://assets.evanta.com/shared/resources/Users/large/anonymous2.jpg"}]}}]}
```

This requests provides a <strong>HTML 200</strong> on success.