Returns a list of all event sponsors.

=
#### Authentication

Declare what authentications are required

Good sample text: The user needs to be logged in and have valid credentials to use this route.

=
#### Parameters

LIST OF ALL PARAMETERS AND WHAT THEY ARE

=
####JSON request example:
```
http://0.0.0.0:3000/ROUTE_NAME
```

=
####JSON response example:

```
{"event_sponsors"=>
  [{"id"=>958,
    "name"=>"Gerhold LLC",
    "description"=>
     "Qui et itaque libero explicabo maiores qui et omnis deserunt modi delectus accusamus id est.",
    "logo"=>"www.example.com/logo.bmp",
    "url"=>"www.example.com",
    "sponsor_type"=>
     {"id"=>4624,
      "name"=>"indigo",
      "description"=>"Multi-channelled tangible monitoring"},
    "event"=>
     {"id"=>6830,
      "name"=>"Ergonomic Concrete Table 23",
      "event_begin_date"=>"2014-03-06",
      "event_end_date"=>"2014-03-07",
      "venue_name"=>"Hyatt Group",
      "address"=>"78526 Gutmann Club",
      "state"=>"TN",
      "postal_code"=>"34958",
      "event_follower_id"=>nil,
      "country"=>{"name"=>"Argentina", "abbreviation"=>"1m2"},
      "group"=>
       {"id"=>8378,
        "name"=>"Open Group 28",
        "description"=>"Open group 28",
        "owner_user_id"=>53763,
        "group_type"=>
         {"id"=>13320, "name"=>"Factory:Open", "description"=>"Open"},
        "owner"=>
         {"id"=>53763,
          "first_name"=>"Aida",
          "last_name"=>"Torp",
          "title"=>"Creator Of All 1",
          "organization_name"=>"Swift, Reilly and Leuschke",
          "photo"=>
           "https://assets.evanta.com/shared/resources/Users/large/anonymous2.jpg",
          "user_role_id"=>53767}}}},
   {"id"=>959,
    "name"=>"Rohan-Raynor",
    "description"=>
     "Cum sunt ab possimus eveniet est architecto error atque et in ullam aperiam quia exercitationem.",
    "logo"=>"www.example.com/logo.bmp",
    "url"=>"www.example.com",
    "sponsor_type"=>
     {"id"=>4624,
      "name"=>"indigo",
      "description"=>"Multi-channelled tangible monitoring"},
    "event"=>
     {"id"=>6831,
      "name"=>"Small Plastic Shirt 24",
      "event_begin_date"=>"2014-03-06",
      "event_end_date"=>"2014-03-07",
      "venue_name"=>"Nikolaus and Sons",
      "address"=>"4738 Mraz Cliffs",
      "state"=>"ME",
      "postal_code"=>"74555-6998",
      "event_follower_id"=>nil,
      "country"=>{"name"=>"Samoa", "abbreviation"=>"1gg"},
      "group"=>
       {"id"=>8379,
        "name"=>"Open Group 29",
        "description"=>"Open group 29",
        "owner_user_id"=>53766,
        "group_type"=>
         {"id"=>13321, "name"=>"Factory:Open", "description"=>"Open"},
        "owner"=>
         {"id"=>53766,
          "first_name"=>"Shad",
          "last_name"=>"Keeling",
          "title"=>"Creator Of All 1",
          "organization_name"=>"Hilpert, Huels and Corwin",
          "photo"=>
           "https://assets.evanta.com/shared/resources/Users/large/anonymous2.jpg",
          "user_role_id"=>53770}}}}]}
```

This requests provides a <strong>HTML 200</strong> on success.