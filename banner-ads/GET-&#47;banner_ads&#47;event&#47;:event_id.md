<!-- --- title: GET /banner_ads/event/:event_id -->

This route pulls all of the banner ads for one particular event.

=
#### Authentication

The user needs to be logged in and have valid credentials to use this route.

=
#### Parameters

:event_id - Integer, passed in through the URL. Derived from the 'id' field of the 'events' table.

=
####JSON request example:
```json
http://0.0.0.0:3000/banner_ads/event/2990
```

=
####JSON response example:
```
{"banner_ads"=>
  [{"id"=>263,
    "graphic_link"=>"www.example.com/graphic_link.jpg",
    "app_sponsor_id"=>nil,
    "link_url"=>"www.example.com",
    "created_by"=>nil,
    "updated_by"=>nil,
    "group"=>nil,
    "event"=>
     {"id"=>2990,
      "name"=>"Fantastic Rubber Gloves",
      "event_begin_date"=>nil,
      "event_end_date"=>nil,
      "venue_name"=>"Volkman LLC",
      "address"=>"52210 Bergnaum Garden",
      "state"=>"AZ",
      "postal_code"=>"89603",
      "event_follower_id"=>nil,
      "country"=>{"name"=>"United States of America", "abbreviation"=>"us"},
      "group"=>
       {"id"=>2858,
        "name"=>"Open Group",
        "description"=>"Open group",
        "owner_user_id"=>nil,
        "app_sponsor_id"=>nil,
        "group_type"=>
         {"id"=>5995, "name"=>"Factory:Open", "description"=>"Open"},
        "owner"=>nil}},
    "event_sponsor"=>nil,
    "app_sponsor"=>nil},
   {"id"=>264,
    "graphic_link"=>"www.example.com/graphic_link.jpg",
    "app_sponsor_id"=>nil,
    "link_url"=>"www.example.com",
    "created_by"=>nil,
    "updated_by"=>nil,
    "group"=>nil,
    "event"=>
     {"id"=>2990,
      "name"=>"Fantastic Rubber Gloves",
      "event_begin_date"=>nil,
      "event_end_date"=>nil,
      "venue_name"=>"Volkman LLC",
      "address"=>"52210 Bergnaum Garden",
      "state"=>"AZ",
      "postal_code"=>"89603",
      "event_follower_id"=>nil,
      "country"=>{"name"=>"United States of America", "abbreviation"=>"us"},
      "group"=>
       {"id"=>2858,
        "name"=>"Open Group",
        "description"=>"Open group",
        "owner_user_id"=>nil,
        "app_sponsor_id"=>nil,
        "group_type"=>
         {"id"=>5995, "name"=>"Factory:Open", "description"=>"Open"},
        "owner"=>nil}},
    "event_sponsor"=>nil,
    "app_sponsor"=>nil}]}
```

This requests provides a <strong>HTML 200</strong> on success.