<!-- --- title: GET /event_sessions/:id -->

Returns all the details for one event session.

=
#### Authentication

The user needs to be logged in and have valid credentials to use this route.

=
#### Parameters

:event_session_id - Integer, passed in through the URL. Derived from the 'id' field 

=
####JSON request example:
```json
http://stage-api-access.evant.com/event_sessions/558
```

=
####JSON response example:
```
{"event_session"=>
  {"id"=>558,
   "name"=>"Intelligent Rubber Shirt",
   "description"=>
    "Compatible 24 hour matrices. Innovative web-enabled projection",
   "start_date_time"=>"2014-02-24T21:26:57.000Z",
   "end_date_time"=>"2014-02-24T22:26:57.000Z",
   "track_name"=>"Polarised multi-state moderator",
   "breakout_id"=>nil,
   "session_type"=>"Practical Plastic Computer",
   "room_name"=>"Fantastic Wooden Table",
   "is_comments_on"=>false,
   "event_speakers"=>[],
   "breakout_session"=>nil,
   "comment_count"=>1,
   "can_add_event_session_to_schedule"=>false,
   "can_add_notes_to_event_sessions"=>false,
   "can_bookmark_event_sessions"=>false,
   "show_event_session_evaluations"=>false,
   "event_session_evaluations"=>[],
   "secret_group_member"=>nil,
   "session_post_likeable"=>false,
   "session_commentable"=>false,
   "event"=>
    {"id"=>4892,
     "name"=>"Fantastic Rubber Gloves 15",
     "event_begin_date"=>nil,
     "event_end_date"=>nil,
     "venue_name"=>"Witting LLC",
     "address"=>"2135 Millie Loop",
     "state"=>"AK",
     "postal_code"=>"90982-9491",
     "event_follower_id"=>nil,
     "country"=>nil,
     "group"=>
      {"id"=>6096,
       "name"=>"Open Group 31",
       "description"=>"Open group 31",
       "owner_user_id"=>nil,
       "group_type"=>
        {"id"=>9491, "name"=>"Factory:Open", "description"=>"Open"},
       "owner"=>nil}},
   "event_sponsor"=>
    {"id"=>738,
     "name"=>"Hermiston and Sons",
     "description"=>
      "At exercitationem illo laboriosam corrupti sit sed inventore similique cupiditate qui voluptatem vitae.",
     "logo"=>nil,
     "url"=>nil,
     "sponsor_type"=>
      {"id"=>3251,
       "name"=>"ivory",
       "description"=>"Enhanced didactic service-desk"}},
   "post"=>
    {"id"=>1381,
     "title"=>"Managed modular neural-net: Small Steel Pants",
     "body"=>
      "---\n- Fugit ut ab eum dolores. Consectetur et molestiae harum officia. Doloremque incidunt\n  et fugit mag
     "body_markdown"=>
      "---\n- Placeat sequi dolorum sapiente saepe animi vitae. Corporis porro architecto cupiditate\n  aliquam ev
     "excerpt"=>"Re-engineered didactic utilisation",
     "thumbnail_teaser_photo"=>"www.example.com/post_thumbnail.jpg",
     "display_rank"=>1,
     "view_count"=>4,
     "show_likes_count"=>false,
     "like_count"=>0,
     "post_likeable"=>false,
     "view_post_likes_list"=>false,
     "post_attachments"=>[],
     "user"=>
      {"id"=>37878,
       "first_name"=>"Franz",
       "last_name"=>"Kohler",
       "title"=>"Random User",
       "organization_name"=>"Fadel, Gleason and Thiel",
       "photo"=>
        "https://assets.evanta.com/shared/resources/Users/large/anonymous2.jpg",
       "user_role_id"=>37880}}}}
```

This requests provides a <strong>HTML 200</strong> on success.