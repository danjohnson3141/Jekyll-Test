<!-- --- title: GET /sponsors/app -->

This returns **all** of the app_sponsors. This means sponsors that are **not** assoicated with any specific groups or events.

=
#### Authentication

The user needs to be logged in and have valid credentials to use this route.

=
#### Parameters

none; default only

=
####JSON request example:
```json
http://stage-api-access.evant.com/sponsors/app
```

=
####JSON response example:

```json
{"sponsors"=>
  [{"id"=>265,
    "name"=>"Greenholt-Konopelski 253",
    "description"=>
     "Aut magni illum sit qui ratione totam nihil aut et voluptatem quis nulla iure.",
    "logo"=>"www.example.com/sponsor_logo.jpg",
    "url"=>"trantowrice.name",
    "splash_sponsor"=>false,
    "sponsor_type"=>
     {"id"=>2,
      "name"=>"lime",
      "description"=>"Persistent incremental extranet",
      "display_rank"=>24},
    "banner_ads"=>
     [{"id"=>50,
       "graphic_link"=>"www.example.com/graphic_link.jpg",
       "link_url"=>"www.example.com"}],
    "event"=>nil,
    "group"=>nil},
   {"id"=>266,
    "name"=>"Gutkowski-Flatley 254",
    "description"=>
     "Numquam laborum autem quos quidem aut dolores perspiciatis voluptatem minus nisi laboriosam.",
    "logo"=>"www.example.com/sponsor_logo.jpg",
    "url"=>"fisherhalvorson.com",
    "splash_sponsor"=>false,
    "sponsor_type"=>
     {"id"=>3,
      "name"=>"orange",
      "description"=>"Re-contextualized mission-critical frame",
      "display_rank"=>24},
    "banner_ads"=>
     [{"id"=>51,
       "graphic_link"=>"www.example.com/graphic_link.jpg",
       "link_url"=>"www.example.com"}],
    "event"=>nil,
    "group"=>nil}]}
```

This requests provides a <strong>HTML 200</strong> on success.