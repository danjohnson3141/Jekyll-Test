This returns **all** the posts associated with one group.

=
#### Authentication

The user needs to be logged in and have valid credentials to use this route.

=
#### Parameters

:group_id - Integer, passed in through the URL. Is derived from the 'id' field on the 'groups' table.

=
####JSON request example:
```
http://0.0.0.0:3000/posts/groups/2197
```

=
####JSON response example:

```
{"posts"=>
  [{"id"=>948,
    "title"=>"Realigned didactic standardization: Practical Concrete Shirt",
    "body"=>
     "---\n- Quae omnis beatae. Reprehenderit quaerat dolorem. Tempora enim cupiditate necessitatibus.\n  Fugit ra
    "body_markdown"=>
     "---\n- Deserunt veniam iste. Ullam rem non ut saepe hic. Rerum ab quo soluta ea dolorum\n  et ipsum. Omnis n
    "excerpt"=>"Open-architected value-added methodology",
    "thumbnail_teaser_photo"=>"www.example.com/post_thumbnail.jpg",
    "display_rank"=>8,
    "view_count"=>0,
    "created_by"=>nil,
    "updated_by"=>nil,
    "group"=>
     {"id"=>2197,
      "name"=>"Ergonomic Plastic Hat",
      "description"=>"Eius maxime quam sequi hic.",
      "owner_user_id"=>10767,
      "app_sponsor_id"=>151,
      "group_type"=>
       {"id"=>4463, "name"=>"Factory:Open", "description"=>"Open"},
      "owner"=>
       {"id"=>10767,
        "first_name"=>"Chadrick",
        "last_name"=>"Mills",
        "title"=>"Creator Of All 1",
        "organization_name"=>"Conn, Klein and Cummerata",
        "photo"=>"www.example.com/user_photo.jpg",
        "user_role_id"=>26821,
        "user_connection_id"=>251}},
    "user"=>
     {"id"=>10770,
      "first_name"=>"Cornelius",
      "last_name"=>"Steuber",
      "title"=>"Random User",
      "organization_name"=>"Pfeffer, Kessler and Walker",
      "photo"=>"www.example.com/user_photo.jpg",
      "user_role_id"=>26822,
      "user_connection_id"=>nil}},
   {"id"=>949,
    "title"=>"Persevering asynchronous installation: Rustic Plastic Computer",
    "body"=>
     "---\n- Non est quo quas magnam unde sunt. Quisquam sit at temporibus ducimus. Odio occaecati\n  tenetur accu
    "body_markdown"=>
     "---\n- Itaque iusto provident et consequatur adipisci sequi. Inventore qui quidem sed qui\n  eum voluptatum 
    "excerpt"=>"Progressive user-facing neural-net",
    "thumbnail_teaser_photo"=>"www.example.com/post_thumbnail.jpg",
    "display_rank"=>7,
    "view_count"=>7,
    "created_by"=>nil,
    "updated_by"=>nil,
    "group"=>
     {"id"=>2197,
      "name"=>"Ergonomic Plastic Hat",
      "description"=>"Eius maxime quam sequi hic.",
      "owner_user_id"=>10767,
      "app_sponsor_id"=>151,
      "group_type"=>
       {"id"=>4463, "name"=>"Factory:Open", "description"=>"Open"},
      "owner"=>
       {"id"=>10767,
        "first_name"=>"Chadrick",
        "last_name"=>"Mills",
        "title"=>"Creator Of All 1",
        "organization_name"=>"Conn, Klein and Cummerata",
        "photo"=>"www.example.com/user_photo.jpg",
        "user_role_id"=>26821,
        "user_connection_id"=>251}},
    "user"=>
     {"id"=>10773,
      "first_name"=>"Ryder",
      "last_name"=>"Zulauf",
      "title"=>"Random User",
      "organization_name"=>"Jenkins, Simonis and Mertz",
      "photo"=>"www.example.com/user_photo.jpg",
      "user_role_id"=>26825,
      "user_connection_id"=>nil}}]}
```

This requests provides a <strong>HTML 200</strong> on success.