<!-- --- title: GET /event_speakers/event/:event_id -->

Returns all of the speakers for one event.

=
####Authentication:

The user needs to be logged in and have valid credentials to use this route.

=
####Parameters:

:event_id - Integer, passed in through the URL. Derived from the 'id' field on the 'events' table.

=
####API request example:
```json
http://stage-api-access.evant.com/event_speakers/event/1947
```

=
####JSON response example:

```json
{"event_speakers"=>
  [{"id"=>97,
    "first_name"=>"Giovanni",
    "last_name"=>"Tillman",
    "title"=>"Intelligent Plastic Hat",
    "organization_name"=>"Ondricka, Dooley and Sporer",
    "bio"=>
     "Minima debitis vel nobis explicabo. Ex officia soluta omnis error fugiat tempora et. Ea dicta voluptatem ius
    "speaker_type"=>"Ergonomic Rubber Computer",
    "moderator"=>true,
    "photo"=>
     "https://assets.evanta.com/shared/resources/Users/large/anonymous2.jpg",
    "user"=>
     {"id"=>14597,
      "email"=>"trea.oberbrunner@bogansipes.info",
      "alt_email"=>"guadalupe@yahoo.com",
      "first_name"=>"Missouri",
      "last_name"=>"Steuber",
      "title"=>"Random User",
      "organization_name"=>"Kris, Kutch and Willms",
      "bio"=>
       "Atque doloremque enim dolorem ut aut earum consequatur et est ut odit corrupti.",
      "photo"=>
       "https://assets.evanta.com/shared/resources/Users/large/anonymous2.jpg",
      "user_role_id"=>14553,
      "user_connection_id"=>nil},
    "event_session"=>
     {"id"=>606,
      "name"=>"Ergonomic Concrete Gloves",
      "description"=>
       "Open-source 24/7 approach. Operative object-oriented challenge",
      "start_date_time"=>"2014-02-26T21:54:54.000Z",
      "end_date_time"=>"2014-02-26T22:54:54.000Z",
      "track_name"=>"Automated multi-tasking data-warehouse",
      "breakout_id"=>nil,
      "session_type"=>"Rustic Granite Shirt",
      "room_name"=>"Incredible Cotton Car",
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
       {"id"=>1947,
        "name"=>"Small Concrete Shirt 120",
        "begin_date"=>"2014-03-08",
        "end_date"=>"2014-03-09",
        "venue_name"=>"Nader-Zieme",
        "address"=>"107 Bins Falls",
        "state"=>"AA",
        "postal_code"=>"72477-4877",
        "event_follower_id"=>nil,
        "country"=>{"name"=>"Marshall Islands", "abbreviation"=>"k0n"},
        "group"=>
         {"id"=>3493,
          "name"=>"Open Group 120",
          "description"=>"Open group 120",
          "owner_user_id"=>14587,
          "group_type"=>
           {"id"=>4599, "name"=>"Factory:Open", "description"=>"Open"},
          "owner"=>
           {"id"=>14587,
            "first_name"=>"Vesta",
            "last_name"=>"Toy",
            "title"=>"Creator Of All 1",
            "organization_name"=>"Herman and Sons",
            "photo"=>
             "https://assets.evanta.com/shared/resources/Users/large/anonymous2.jpg",
            "user_role_id"=>14543,
            "user_connection_id"=>nil}}},
      "event_sponsor"=>
       {"id"=>662,
        "name"=>"Larson Inc",
        "description"=>
         "Rerum officia quis impedit quos totam in corrupti consectetur adipisci voluptatem quo inventore animi.",
        "logo"=>"www.example.com/logo.bmp",
        "url"=>"www.example.com",
        "sponsor_type"=>
         {"id"=>3531,
          "name"=>"cyan",
          "description"=>"Multi-lateral zero tolerance challenge"}},
      "post"=>
       {"id"=>826,
        "title"=>"Advanced fresh-thinking focus group: Sleek Plastic Hat",
        "body"=>
         "---\n- Et mollitia repellat veritatis est. Enim doloribus illum deserunt vel et. Corrupti\n  placeat pro
        "body_markdown"=>
         "---\n- Quo fugit et ea. Ut id aut. Eum dolore voluptatum commodi possimus voluptatibus\n  cupiditate. Ve
        "excerpt"=>"Intuitive 4th generation software",
        "thumbnail_teaser_photo"=>"www.example.com/post_thumbnail.jpg",
        "display_rank"=>6,
        "view_count"=>5,
        "show_likes_count"=>true,
        "like_count"=>0,
        "post_likes"=>true,
        "show_post_likes_list"=>true,
        "post_attachments"=>[],
        "user"=>
         {"id"=>14590,
          "first_name"=>"Vernice",
          "last_name"=>"Dickinson",
          "title"=>"Random User",
          "organization_name"=>"Konopelski-Ernser",
          "photo"=>
           "https://assets.evanta.com/shared/resources/Users/large/anonymous2.jpg",
          "user_role_id"=>14546,
          "user_connection_id"=>nil}},
      "event_speakers"=>
       [{"id"=>97,
         "user_id"=>14597,
         "first_name"=>"Giovanni",
         "last_name"=>"Tillman",
         "title"=>"Intelligent Plastic Hat",
         "organization_name"=>"Ondricka, Dooley and Sporer",
         "bio"=>
          "Minima debitis vel nobis explicabo. Ex officia soluta omnis error fugiat tempora et. Ea dicta voluptate
         "speaker_type"=>"Ergonomic Rubber Computer",
         "moderator"=>true,
         "photo"=>
          "https://assets.evanta.com/shared/resources/Users/large/anonymous2.jpg"},
        {"id"=>98,
         "user_id"=>14598,
         "first_name"=>"Jacinthe",
         "last_name"=>"Raynor",
         "title"=>"Ergonomic Concrete Chair",
         "organization_name"=>"Ritchie, Ullrich and Rempel",
         "bio"=>
          "Cumque saepe et. Est debitis et enim earum. Nam in nemo ipsa. Minus dignissimos facere dolores amet sun
         "speaker_type"=>"Sleek Granite Hat",
         "moderator"=>true,
         "photo"=>
          "https://assets.evanta.com/shared/resources/Users/large/anonymous2.jpg"}]}},
   {"id"=>98,
    "first_name"=>"Jacinthe",
    "last_name"=>"Raynor",
    "title"=>"Ergonomic Concrete Chair",
    "organization_name"=>"Ritchie, Ullrich and Rempel",
    "bio"=>
     "Cumque saepe et. Est debitis et enim earum. Nam in nemo ipsa. Minus dignissimos facere dolores amet sunt.\n\
    "speaker_type"=>"Sleek Granite Hat",
    "moderator"=>true,
    "photo"=>
     "https://assets.evanta.com/shared/resources/Users/large/anonymous2.jpg",
    "user"=>
     {"id"=>14598,
      "email"=>"golden@osinski.info",
      "alt_email"=>"tyreek@hotmail.com",
      "first_name"=>"Devante",
      "last_name"=>"Bahringer",
      "title"=>"Random User",
      "organization_name"=>"Legros, Hammes and Jones",
      "bio"=>
       "Dolores exercitationem in labore debitis est repellendus voluptas ab voluptatibus iste commodi.",
      "photo"=>
       "https://assets.evanta.com/shared/resources/Users/large/anonymous2.jpg",
      "user_role_id"=>14554,
      "user_connection_id"=>nil},
    "event_session"=>
     {"id"=>606,
      "name"=>"Ergonomic Concrete Gloves",
      "description"=>
       "Open-source 24/7 approach. Operative object-oriented challenge",
      "start_date_time"=>"2014-02-26T21:54:54.000Z",
      "end_date_time"=>"2014-02-26T22:54:54.000Z",
      "track_name"=>"Automated multi-tasking data-warehouse",
      "breakout_id"=>nil,
      "session_type"=>"Rustic Granite Shirt",
      "room_name"=>"Incredible Cotton Car",
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
       {"id"=>1947,
        "name"=>"Small Concrete Shirt 120",
        "begin_date"=>"2014-03-08",
        "end_date"=>"2014-03-09",
        "venue_name"=>"Nader-Zieme",
        "address"=>"107 Bins Falls",
        "state"=>"AA",
        "postal_code"=>"72477-4877",
        "event_follower_id"=>nil,
        "country"=>{"name"=>"Marshall Islands", "abbreviation"=>"k0n"},
        "group"=>
         {"id"=>3493,
          "name"=>"Open Group 120",
          "description"=>"Open group 120",
          "owner_user_id"=>14587,
          "group_type"=>
           {"id"=>4599, "name"=>"Factory:Open", "description"=>"Open"},
          "owner"=>
           {"id"=>14587,
            "first_name"=>"Vesta",
            "last_name"=>"Toy",
            "title"=>"Creator Of All 1",
            "organization_name"=>"Herman and Sons",
            "photo"=>
             "https://assets.evanta.com/shared/resources/Users/large/anonymous2.jpg",
            "user_role_id"=>14543,
            "user_connection_id"=>nil}}},
      "event_sponsor"=>
       {"id"=>662,
        "name"=>"Larson Inc",
        "description"=>
         "Rerum officia quis impedit quos totam in corrupti consectetur adipisci voluptatem quo inventore animi.",
        "logo"=>"www.example.com/logo.bmp",
        "url"=>"www.example.com",
        "sponsor_type"=>
         {"id"=>3531,
          "name"=>"cyan",
          "description"=>"Multi-lateral zero tolerance challenge"}},
      "post"=>
       {"id"=>826,
        "title"=>"Advanced fresh-thinking focus group: Sleek Plastic Hat",
        "body"=>
         "---\n- Et mollitia repellat veritatis est. Enim doloribus illum deserunt vel et. Corrupti\n  placeat pro
        "body_markdown"=>
         "---\n- Quo fugit et ea. Ut id aut. Eum dolore voluptatum commodi possimus voluptatibus\n  cupiditate. Ve
        "excerpt"=>"Intuitive 4th generation software",
        "thumbnail_teaser_photo"=>"www.example.com/post_thumbnail.jpg",
        "display_rank"=>6,
        "view_count"=>5,
        "show_likes_count"=>true,
        "like_count"=>0,
        "post_likes"=>true,
        "show_post_likes_list"=>true,
        "post_attachments"=>[],
        "user"=>
         {"id"=>14590,
          "first_name"=>"Vernice",
          "last_name"=>"Dickinson",
          "title"=>"Random User",
          "organization_name"=>"Konopelski-Ernser",
          "photo"=>
           "https://assets.evanta.com/shared/resources/Users/large/anonymous2.jpg",
          "user_role_id"=>14546,
          "user_connection_id"=>nil}},
      "event_speakers"=>
       [{"id"=>97,
         "user_id"=>14597,
         "first_name"=>"Giovanni",
         "last_name"=>"Tillman",
         "title"=>"Intelligent Plastic Hat",
         "organization_name"=>"Ondricka, Dooley and Sporer",
         "bio"=>
          "Minima debitis vel nobis explicabo. Ex officia soluta omnis error fugiat tempora et. Ea dicta voluptate
         "speaker_type"=>"Ergonomic Rubber Computer",
         "moderator"=>true,
         "photo"=>
          "https://assets.evanta.com/shared/resources/Users/large/anonymous2.jpg"},
        {"id"=>98,
         "user_id"=>14598,
         "first_name"=>"Jacinthe",
         "last_name"=>"Raynor",
         "title"=>"Ergonomic Concrete Chair",
         "organization_name"=>"Ritchie, Ullrich and Rempel",
         "bio"=>
          "Cumque saepe et. Est debitis et enim earum. Nam in nemo ipsa. Minus dignissimos facere dolores amet sun
         "speaker_type"=>"Sleek Granite Hat",
         "moderator"=>true,
         "photo"=>
          "https://assets.evanta.com/shared/resources/Users/large/anonymous2.jpg"}]}}]}

```

This requests provides a <strong>HTML 200</strong> on success.