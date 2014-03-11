<!-- --- title: GET /event_users/events/:user_id -->

This returns all the event users for one event.

=
#### Authentication

The user needs to be logged in and have valid credentials to use this route.

=
#### Parameters

LIST OF ALL PARAMETERS AND WHAT THEY ARE

=
####JSON request example:
```
http://0.0.0.0:3000/event_users/events/9675
```

=
####JSON response example:

```json
{"event_users"=>
  [{"id"=>3144,
    "event_registration_status"=>{"id"=>767, "key"=>"registered"},
    "event"=>
     {"id"=>9675,
      "name"=>"Incredible Granite Table 55",
      "event_begin_date"=>"2014-03-06",
      "event_end_date"=>"2014-03-07",
      "venue_name"=>"Wilkinson LLC",
      "address"=>"321 Schinner Overpass",
      "state"=>"OH",
      "postal_code"=>"85180-6288",
      "event_follower_id"=>2149,
      "country"=>{"name"=>"Uganda", "abbreviation"=>"sz6"},
      "group"=>
       {"id"=>11641,
        "name"=>"Incredible Wooden Shoes",
        "description"=>
         "Voluptas deserunt aut tenetur iusto quisquam unde cupiditate hic id.",
        "owner_user_id"=>76059,
        "group_type"=>
         {"id"=>18301, "name"=>"Factory:Open", "description"=>"Open"},
        "owner"=>
         {"id"=>76059,
          "first_name"=>"Jonatan",
          "last_name"=>"Okuneva",
          "title"=>"Creator Of All 1",
          "organization_name"=>"Klein Group",
          "photo"=>
           "https://assets.evanta.com/shared/resources/Users/large/anonymous2.jpg",
          "user_role_id"=>76063}}},
    "event_sponsor"=>
     {"id"=>1354,
      "name"=>"Lemke, Deckow and Reilly",
      "description"=>
       "Rerum est aspernatur sint odit incidunt molestiae distinctio quas doloribus qui et error.",
      "logo"=>"www.example.com/logo.bmp",
      "url"=>"www.example.com",
      "sponsor_type"=>
       {"id"=>7306,
        "name"=>"salmon",
        "description"=>"Self-enabling object-oriented pricing structure"},
      "event"=>
       {"id"=>9675,
        "name"=>"Incredible Granite Table 55",
        "event_begin_date"=>"2014-03-06",
        "event_end_date"=>"2014-03-07",
        "venue_name"=>"Wilkinson LLC",
        "address"=>"321 Schinner Overpass",
        "state"=>"OH",
        "postal_code"=>"85180-6288",
        "event_follower_id"=>2149,
        "country"=>{"name"=>"Uganda", "abbreviation"=>"sz6"},
        "group"=>
         {"id"=>11641,
          "name"=>"Incredible Wooden Shoes",
          "description"=>
           "Voluptas deserunt aut tenetur iusto quisquam unde cupiditate hic id.",
          "owner_user_id"=>76059,
          "group_type"=>
           {"id"=>18301, "name"=>"Factory:Open", "description"=>"Open"},
          "owner"=>
           {"id"=>76059,
            "first_name"=>"Jonatan",
            "last_name"=>"Okuneva",
            "title"=>"Creator Of All 1",
            "organization_name"=>"Klein Group",
            "photo"=>
             "https://assets.evanta.com/shared/resources/Users/large/anonymous2.jpg",
            "user_role_id"=>76063}}}}},
   {"id"=>3145,
    "event_registration_status"=>{"id"=>768, "key"=>"attended"},
    "event"=>
     {"id"=>9676,
      "name"=>"Gorgeous Concrete Table 56",
      "event_begin_date"=>"2014-03-06",
      "event_end_date"=>"2014-03-07",
      "venue_name"=>"Crooks and Sons",
      "address"=>"24022 Haylie Port",
      "state"=>"AS",
      "postal_code"=>"31728-4187",
      "event_follower_id"=>2150,
      "country"=>{"name"=>"Liechtenstein", "abbreviation"=>"b0p"},
      "group"=>
       {"id"=>11641,
        "name"=>"Incredible Wooden Shoes",
        "description"=>
         "Voluptas deserunt aut tenetur iusto quisquam unde cupiditate hic id.",
        "owner_user_id"=>76059,
        "group_type"=>
         {"id"=>18301, "name"=>"Factory:Open", "description"=>"Open"},
        "owner"=>
         {"id"=>76059,
          "first_name"=>"Jonatan",
          "last_name"=>"Okuneva",
          "title"=>"Creator Of All 1",
          "organization_name"=>"Klein Group",
          "photo"=>
           "https://assets.evanta.com/shared/resources/Users/large/anonymous2.jpg",
          "user_role_id"=>76063}}},
    "event_sponsor"=>
     {"id"=>1355,
      "name"=>"Mitchell-Weissnat",
      "description"=>
       "Exercitationem consequuntur aspernatur id quisquam quam quo libero ut officia ipsa.",
      "logo"=>"www.example.com/logo.bmp",
      "url"=>"www.example.com",
      "sponsor_type"=>
       {"id"=>7307,
        "name"=>"grey",
        "description"=>"Enterprise-wide 24 hour attitude"},
      "event"=>
       {"id"=>9676,
        "name"=>"Gorgeous Concrete Table 56",
        "event_begin_date"=>"2014-03-06",
        "event_end_date"=>"2014-03-07",
        "venue_name"=>"Crooks and Sons",
        "address"=>"24022 Haylie Port",
        "state"=>"AS",
        "postal_code"=>"31728-4187",
        "event_follower_id"=>2150,
        "country"=>{"name"=>"Liechtenstein", "abbreviation"=>"b0p"},
        "group"=>
         {"id"=>11641,
          "name"=>"Incredible Wooden Shoes",
          "description"=>
           "Voluptas deserunt aut tenetur iusto quisquam unde cupiditate hic id.",
          "owner_user_id"=>76059,
          "group_type"=>
           {"id"=>18301, "name"=>"Factory:Open", "description"=>"Open"},
          "owner"=>
           {"id"=>76059,
            "first_name"=>"Jonatan",
            "last_name"=>"Okuneva",
            "title"=>"Creator Of All 1",
            "organization_name"=>"Klein Group",
            "photo"=>
             "https://assets.evanta.com/shared/resources/Users/large/anonymous2.jpg",
            "user_role_id"=>76063}}}}}]}
```

This requests provides a <strong>HTML 200</strong> on success.