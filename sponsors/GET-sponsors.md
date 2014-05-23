<!-- --- title: GET /sponsors -->

This retruns a list of **all** sponsors, regardless of any other associations they might have.

=
####Authentication:

The user needs to be logged in and have valid credentials to use this route.

=
####Parameters:

None; default only.

=
####API request example:
```html
http://stage-api-access.evant.com/sponsors
```

=
####JSON response example:

```json
{"sponsors"=>
  [{"id"=>477,
    "name"=>"Marvin-Jacobs 1",
    "description"=>
     "Hic repellendus harum ut molestiae quo rerum eaque voluptas voluptatem est qui consequuntur repudiandae pers
    "logo"=>"www.example.com/sponsor_logo.jpg",
    "url"=>"stoltenberg.biz",
    "splash_sponsor"=>false,
    "sponsor_type"=>
     {"id"=>13,
      "name"=>"turquoise",
      "description"=>"Public-key methodical Graphic Interface",
      "display_rank"=>26},
    "banner_ads"=>
     [{"id"=>170,
       "graphic_link"=>"www.example.com/graphic_link.jpg",
       "link_url"=>"www.example.com"}],
    "event"=>nil,
    "group"=>nil},
   {"id"=>478,
    "name"=>"Kihn Group 2",
    "description"=>
     "Aliquid deleniti et repellat possimus qui in rerum omnis quia quaerat atque facere rerum.",
    "logo"=>"www.example.com/sponsor_logo.jpg",
    "url"=>"kihn.org",
    "splash_sponsor"=>false,
    "sponsor_type"=>
     {"id"=>2,
      "name"=>"orchid",
      "description"=>"Profit-focused radical challenge",
      "display_rank"=>26},
    "banner_ads"=>
     [{"id"=>171,
       "graphic_link"=>"www.example.com/graphic_link.jpg",
       "link_url"=>"www.example.com"}],
    "event"=>nil,
    "group"=>nil},
   {"id"=>479,
    "name"=>"McGlynn, Bernier and Huel 3",
    "description"=>
     "Excepturi unde tenetur repellat necessitatibus sint culpa perspiciatis iusto veritatis.",
    "logo"=>"www.example.com/sponsor_logo.jpg",
    "url"=>"gleason.com",
    "splash_sponsor"=>false,
    "sponsor_type"=>
     {"id"=>3,
      "name"=>"salmon",
      "description"=>"Public-key upward-trending customer loyalty",
      "display_rank"=>26},
    "banner_ads"=>
     [{"id"=>172,
       "graphic_link"=>"www.example.com/graphic_link.jpg",
       "link_url"=>"www.example.com"}],
    "event"=>nil,
    "group"=>
     {"id"=>865,
      "name"=>"Fantastic Granite Shirt 1",
      "group_type_name"=>"Factory:Open"}},
   {"id"=>480,
    "name"=>"McLaughlin, Marks and Huels 4",
    "description"=>
     "Vitae id libero corporis laborum est vero ut deleniti aut accusantium ab soluta reprehenderit qui.",
    "logo"=>"www.example.com/sponsor_logo.jpg",
    "url"=>"ruel.biz",
    "splash_sponsor"=>false,
    "sponsor_type"=>
     {"id"=>3,
      "name"=>"red",
      "description"=>"Switchable holistic archive",
      "display_rank"=>26},
    "banner_ads"=>
     [{"id"=>173,
       "graphic_link"=>"www.example.com/graphic_link.jpg",
       "link_url"=>"www.example.com"}],
    "event"=>nil,
    "group"=>
     {"id"=>866,
      "name"=>"Ergonomic Concrete Hat 2",
      "group_type_name"=>"Factory:Open"}},
   {"id"=>481,
    "name"=>"Haag-Lebsack 5",
    "description"=>
     "Magni exercitationem provident architecto consequatur mollitia ad earum omnis fugit omnis error ut sint quia
    "logo"=>"www.example.com/sponsor_logo.jpg",
    "url"=>"stracke.net",
    "splash_sponsor"=>false,
    "sponsor_type"=>
     {"id"=>12,
      "name"=>"orange",
      "description"=>"Virtual assymetric help-desk",
      "display_rank"=>26},
    "banner_ads"=>
     [{"id"=>174,
       "graphic_link"=>"www.example.com/graphic_link.jpg",
       "link_url"=>"www.example.com"}],
    "event"=>{"id"=>545, "name"=>"Ergonomic Steel Pants 6"},
    "group"=>nil},
   {"id"=>482,
    "name"=>"Jacobson, Marvin and Stracke 6",
    "description"=>
     "Ad ut sit sit perspiciatis molestias voluptate saepe officiis est minima.",
    "logo"=>"www.example.com/sponsor_logo.jpg",
    "url"=>"schinneryundt.info",
    "splash_sponsor"=>false,
    "sponsor_type"=>
     {"id"=>1,
      "name"=>"red",
      "description"=>"Vision-oriented transitional infrastructure",
      "display_rank"=>26},
    "banner_ads"=>
     [{"id"=>175,
       "graphic_link"=>"www.example.com/graphic_link.jpg",
       "link_url"=>"www.example.com"}],
    "event"=>{"id"=>546, "name"=>"Rustic Plastic Table 7"},
    "group"=>nil}]}
```

This requests provides a <strong>HTML 200</strong> on success.