<!-- --- title: GET /sponsors/:id -->

This returns **one** data record relating to a sponsor as defined by the ID passed in.

=
#### Authentication

The user needs to be logged in and have valid credentials to use this route.

=
#### Parameters

(sponsor) :id - Integer, passed in through the URL. Is derived from the 'id' field on the the 'app_sponsors' table.

=
####JSON request example:
```json
http://0.0.0.0:3000/sponsors/11
```

=
####JSON response example:

```json
{"sponsor"=>
  {"id"=>11,
   "name"=>"Lowe, Ratke and Bins 11",
   "description"=>
    "Deleniti magnam dolorem enim commodi voluptatem sed velit et nemo.",
   "logo"=>"www.example.com/sponsor_logo.jpg",
   "url"=>"miller.info",
   "splash_sponsor"=>false,
   "sponsor_type"=>
    {"id"=>11,
     "name"=>"gold",
     "description"=>"Cloned object-oriented help-desk",
     "display_rank"=>45},
   "banner_ads"=>
    [{"id"=>11,
      "graphic_link"=>"www.example.com/graphic_link.jpg",
      "link_url"=>"www.example.com"}],
   "event"=>{"id"=>1, "name"=>"Intelligent Rubber Shoes 1"},
   "group"=>nil}}
```

This requests provides a <strong>HTML 200</strong> on success.