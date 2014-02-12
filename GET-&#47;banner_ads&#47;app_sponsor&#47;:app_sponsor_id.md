This route pulls all of the banner ads for one particular sponsor

Declare what authentications are required

Good sample text: The user needs to be logged in and have valid credentials to use this route.

#### Parameters

:app_sponsor_id
This is passed in the URL and is derived from the 'id' field on the the 'app_sponsors' table.

=

####JSON request example:
```
http://0.0.0.0:3000/ROUTE_NAME
```
=
####JSON response example:

```
{"banner_ads"=>
  [{"id"=>207,
    "graphic_link"=>"www.example.com/graphic_link.jpg",
    "app_sponsor_id"=>171,
    "link_url"=>"www.example.com",
    "created_by"=>nil,
    "updated_by"=>nil,
    "group"=>nil,
    "event"=>nil,
    "event_sponsor"=>nil,
    "app_sponsor"=>
     {"id"=>171,
      "name"=>"Wuckert, Herman and Pacocha",
      "description"=>
       "Explicabo non recusandae omnis dolores rem esse est iste excepturi et enim minus atque ab.",
      "logo"=>nil,
      "url"=>nil,
      "sponsor_type"=>
       {"id"=>239,
        "name"=>"A type of Sponsor",
        "description"=>"A Sponsor Type"},
      "users"=>[]}},
   {"id"=>208,
    "graphic_link"=>"www.example.com/graphic_link.jpg",
    "app_sponsor_id"=>171,
    "link_url"=>"www.example.com",
    "created_by"=>nil,
    "updated_by"=>nil,
    "group"=>nil,
    "event"=>nil,
    "event_sponsor"=>nil,
    "app_sponsor"=>
     {"id"=>171,
      "name"=>"Wuckert, Herman and Pacocha",
      "description"=>
       "Explicabo non recusandae omnis dolores rem esse est iste excepturi et enim minus atque ab.",
      "logo"=>nil,
      "url"=>nil,
      "sponsor_type"=>
       {"id"=>239,
        "name"=>"A type of Sponsor",
        "description"=>"A Sponsor Type"},
      "users"=>[]}}]}
```

This requests provides a HTML RESPONSE NUMBER on success.