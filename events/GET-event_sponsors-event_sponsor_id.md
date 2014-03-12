<!-- --- title: GET /event_sponsors/:event_sponsor_id -->

Returns information on one event sponsor.

=
#### Authentication

The user needs to be logged in and have valid credentials to use this route.

=
#### Parameters

:event_sponsor_id - Integer, passed in through the URL. Is derived from the 'id' field on the 'event_sponsors' table.

=
####JSON request example:
```json
http://0.0.0.0:3000/event_sponsors/2056
```

=
####JSON response example:

```json
{"event_sponsor"=>
  {"id"=>2056,
   "name"=>"Baumbach-King",
   "description"=>
    "Molestias rerum quia odit provident sunt at ut temporibus sint accusantium animi numquam nihil enim.",
   "logo"=>"www.example.com/logo.bmp",
   "url"=>"www.example.com",
   "sponsor_type"=>
    {"id"=>11988,
     "name"=>"orange",
     "description"=>"Face to face human-resource moderator"},
   "event"=>
    {"id"=>14481,
     "name"=>"Ergonomic Plastic Shoes 54",
     "event_begin_date"=>"2014-03-07",
     "event_end_date"=>"2014-03-08",
     "venue_name"=>"Schumm-Heaney",
     "address"=>"586 Torphy Tunnel",
     "state"=>"SD",
     "postal_code"=>"77210",
     "event_follower_id"=>3261,
     "country"=>
      {"name"=>"Saint Vincent and the Grenadines", "abbreviation"=>"w79"},
     "group"=>
      {"id"=>17228,
       "name"=>"Open Group 70",
       "description"=>"Open group 70",
       "owner_user_id"=>112896,
       "group_type"=>
        {"id"=>26833, "name"=>"Factory:Open", "description"=>"Open"},
       "owner"=>
        {"id"=>112896,
         "first_name"=>"Darren",
         "last_name"=>"Lebsack",
         "title"=>"Creator Of All 1",
         "organization_name"=>"Breitenberg, Stanton and Thiel",
         "photo"=>
          "https://assets.evanta.com/shared/resources/Users/large/anonymous2.jpg",
         "user_role_id"=>112900}}}}}
```

This requests provides a <strong>HTML 200</strong> on success.