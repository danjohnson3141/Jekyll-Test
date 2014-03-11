<!-- --- title: GET /event_speakers/:event_speaker_id -->

Returns information for one event speaker.

=
#### Authentication

The user needs to be logged in and have valid credentials to use this route.

=
#### Parameters

:event_speaker_id - Integer, passed in through the URL. Is derived from the 'id' field on the 'event_speaker' table.

=
####JSON request example:
```json
http://0.0.0.0:3000/event_speakers/61
```

=
####JSON response example:

```json
{"event_speaker"=>
  {"id"=>61,
   "first_name"=>"Carolyn",
   "last_name"=>"Schoen",
   "title"=>"Rustic Wooden Computer",
   "organization_name"=>"Abbott-DuBuque",
   "bio"=>
    "Qui voluptatem dolor adipisci. Rem pariatur aut necessitatibus velit. Dolore cupiditate illum porro ratione.\
   "speaker_type"=>"Intelligent Steel Car",
   "moderator"=>true,
   "photo"=>
    "https://assets.evanta.com/shared/resources/Users/large/anonymous2.jpg",
   "user"=>
    {"id"=>8496,
     "email"=>"rosalee@hudson.name",
     "alt_email"=>"mina@yahoo.com",
     "first_name"=>"Ezequiel",
     "last_name"=>"Hodkiewicz",
     "title"=>"Random User",
     "organization_name"=>"Block, Bayer and Dickens",
     "bio"=>
      "Repudiandae odio ut quia ut accusantium id nihil maxime voluptatem quo et.",
     "photo"=>
      "https://assets.evanta.com/shared/resources/Users/large/anonymous2.jpg",
     "user_role_id"=>8476,
     "user_connection_id"=>nil},
   "event_session"=>
    {"id"=>359,
     "name"=>"Intelligent Plastic Gloves",
     "description"=>
      "Persevering zero administration definition. Enhanced eco-centric archive",
     "start_date_time"=>"2014-02-26T21:26:31.000Z",
     "end_date_time"=>"2014-02-26T22:26:31.000Z",
     "track_name"=>"Triple-buffered explicit task-force",
     "breakout_id"=>nil,
     "session_type"=>"Incredible Concrete Shirt",
     "room_name"=>"Fantastic Cotton Hat",
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
      {"id"=>1121,
       "name"=>"Intelligent Cotton Shoes 38",
       "begin_date"=>"2014-03-08",
       "end_date"=>"2014-03-09",
       "venue_name"=>"Mertz-Hagenes",
       "address"=>"11468 Marvin Motorway",
       "state"=>"MN",
       "postal_code"=>"34251",
       "event_follower_id"=>nil,
       "country"=>{"name"=>"Vanuatu", "abbreviation"=>"ym8"},
       "group"=>
        {"id"=>2041,
         "name"=>"Open Group 39",
         "description"=>"Open group 39",
         "owner_user_id"=>8497,
         "group_type"=>
          {"id"=>2682, "name"=>"Factory:Open", "description"=>"Open"},
         "owner"=>
          {"id"=>8497,
           "first_name"=>"Roberto",
           "last_name"=>"Paucek",
           "title"=>"Creator Of All 1",
           "organization_name"=>"Breitenberg, Leannon and Gottlieb",
           "photo"=>
            "https://assets.evanta.com/shared/resources/Users/large/anonymous2.jpg",
           "user_role_id"=>8477,
           "user_connection_id"=>nil}}},
     "event_sponsor"=>
      {"id"=>397,
       "name"=>"Ortiz LLC",
       "description"=>
        "Enim animi ipsam provident in repellendus mollitia omnis voluptas quo minus recusandae voluptatem dolorem
       "logo"=>"www.example.com/logo.bmp",
       "url"=>"www.example.com",
       "sponsor_type"=>
        {"id"=>2066,
         "name"=>"pink",
         "description"=>"Programmable high-level throughput"}},
     "post"=>
      {"id"=>496,
       "title"=>
        "Re-contextualized background capability: Ergonomic Granite Gloves",
       "body"=>
        "---\n- Et ullam ea aut et ipsam hic. Temporibus asperiores repellat aut vero cum sit aliquam.\n  Adipisci
       "body_markdown"=>
        "---\n- Beatae et repudiandae et. Dolorum voluptatem molestiae. Beatae aut consequatur vel\n  aliquid labo
       "excerpt"=>"Stand-alone 4th generation concept",
       "thumbnail_teaser_photo"=>"www.example.com/post_thumbnail.jpg",
       "display_rank"=>2,
       "view_count"=>5,
       "show_likes_count"=>true,
       "like_count"=>0,
       "post_likes"=>true,
       "show_post_likes_list"=>true,
       "post_attachments"=>[],
       "user"=>
        {"id"=>8500,
         "first_name"=>"Larissa",
         "last_name"=>"Koelpin",
         "title"=>"Random User",
         "organization_name"=>"Green, Bradtke and Schmitt",
         "photo"=>
          "https://assets.evanta.com/shared/resources/Users/large/anonymous2.jpg",
         "user_role_id"=>8480,
         "user_connection_id"=>nil}},
     "event_speakers"=>
      [{"id"=>61,
        "user_id"=>8496,
        "first_name"=>"Carolyn",
        "last_name"=>"Schoen",
        "title"=>"Rustic Wooden Computer",
        "organization_name"=>"Abbott-DuBuque",
        "bio"=>
         "Qui voluptatem dolor adipisci. Rem pariatur aut necessitatibus velit. Dolore cupiditate illum porro rati
        "speaker_type"=>"Intelligent Steel Car",
        "moderator"=>true,
        "photo"=>
         "https://assets.evanta.com/shared/resources/Users/large/anonymous2.jpg"}]}}}
```

This requests provides a <strong>HTML 200</strong> on success.