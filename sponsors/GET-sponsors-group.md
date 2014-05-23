<!-- --- title: GET /sponsors/group -->

Returns a list of **all** sponsors that have been associated with specific groups.

=
####Authentication:

The user needs to be logged in and have valid credentials to use this route.

=
####Parameters:

None; default only.

=
####API request example:
```html
http://stage-api-access.evant.com/sponsors/group
```

=
####JSON response example:

```json
{"sponsors"=>
  [{"id"=>470,
    "name"=>"Walsh-Heidenreich 6",
    "description"=>
     "Dolor eligendi ullam voluptatibus consequatur quasi quo facilis est quas.",
    "logo"=>"www.example.com/sponsor_logo.jpg",
    "url"=>"price.info",
    "splash_sponsor"=>false,
    "sponsor_type"=>
     {"id"=>4,
      "name"=>"blue",
      "description"=>"Polarised mission-critical open system",
      "display_rank"=>10},
    "banner_ads"=>
     [{"id"=>163,
       "graphic_link"=>"www.example.com/graphic_link.jpg",
       "link_url"=>"www.example.com"}],
    "event"=>nil,
    "group"=>
     {"id"=>853,
      "name"=>"Incredible Rubber Table 1",
      "group_type_name"=>"Factory:Open"}},
   {"id"=>471,
    "name"=>"Trantow, Pouros and Kuhic 7",
    "description"=>
     "Sint iusto optio sequi quo autem sit vel dolores ipsa non tenetur saepe.",
    "logo"=>"www.example.com/sponsor_logo.jpg",
    "url"=>"kreigerjohns.org",
    "splash_sponsor"=>false,
    "sponsor_type"=>
     {"id"=>2,
      "name"=>"ivory",
      "description"=>"Multi-tiered mobile ability",
      "display_rank"=>10},
    "banner_ads"=>
     [{"id"=>164,
       "graphic_link"=>"www.example.com/graphic_link.jpg",
       "link_url"=>"www.example.com"}],
    "event"=>nil,
    "group"=>
     {"id"=>854,
      "name"=>"Incredible Steel Shirt 2",
      "group_type_name"=>"Factory:Open"}}]}
```

This requests provides a <strong>HTML 200</strong> on success.