<!-- --- title: GET /sponsors/event -->

This returns a list of **all** the sponsors that have been associated with an event. 

=
#### Authentication

The user needs to be logged in and have valid credentials to use this route.

=
#### Parameters

none; default only

=
####API request example:
```json
http://stage-api-access.evant.com/sponsors/event
```

=
####JSON response example:

```json
{"sponsors"=>
  [{"id"=>463,
    "name"=>"Walter, Kessler and Nitzsche 71",
    "description"=>
     "Dolore in beatae distinctio ducimus dolores magnam voluptatibus voluptates non aut aspernatur non qui voluptas.",
    "logo"=>"www.example.com/sponsor_logo.jpg",
    "url"=>"donnelly.biz",
    "splash_sponsor"=>false,
    "sponsor_type"=>
     {"id"=>4,
      "name"=>"plum",
      "description"=>"Future-proofed responsive hardware",
      "display_rank"=>54},
    "banner_ads"=>
     [{"id"=>156,
       "graphic_link"=>"www.example.com/graphic_link.jpg",
       "link_url"=>"www.example.com"}],
    "event"=>{"id"=>528, "name"=>"Gorgeous Wooden Pants 11"},
    "group"=>nil},
   {"id"=>464,
    "name"=>"Leffler-Vandervort 72",
    "description"=>
     "Beatae et dolorem incidunt veniam illo quaerat nulla et commodi nesciunt nostrum velit porro ea.",
    "logo"=>"www.example.com/sponsor_logo.jpg",
    "url"=>"ledner.org",
    "splash_sponsor"=>false,
    "sponsor_type"=>
     {"id"=>5,
      "name"=>"pink",
      "description"=>"Versatile analyzing migration",
      "display_rank"=>54},
    "banner_ads"=>
     [{"id"=>157,
       "graphic_link"=>"www.example.com/graphic_link.jpg",
       "link_url"=>"www.example.com"}],
    "event"=>{"id"=>529, "name"=>"Fantastic Granite Pants 12"},
    "group"=>nil}]}
```

This requests provides a <strong>HTML 200</strong> on success.