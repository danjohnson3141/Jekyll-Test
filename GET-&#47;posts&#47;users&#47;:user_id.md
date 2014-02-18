Returns all of the posts from a single user

=
#### Authentication

The user needs to be logged in and have valid credentials to use this route.

=
#### Parameters

:user_id

This is passed in through the URL. It is derived from the 'id' field on the 'users' table.

=
####JSON request example:
```
http://0.0.0.0:3000/posts/users/13935
```

=
####JSON response example:

```
{"posts"=>
  [{"id"=>1056,
    "title"=>"Synergized methodical utilisation: Gorgeous Granite Pants",
    "body"=>
     "---\n- Possimus architecto iure cum. Commodi qui ut rem. Optio consectetur praesentium\n  vel deserunt offic
    "body_markdown"=>
     "---\n- At vel modi non aliquam architecto. Sequi vero ab soluta sit maiores. Magnam voluptatem\n  mollitia u
    "excerpt"=>"Optional zero tolerance access",
    "thumbnail_teaser_photo"=>"www.example.com/post_thumbnail.jpg",
    "display_rank"=>4,
    "view_count"=>6,
    "created_by"=>nil,
    "updated_by"=>nil,
    "group"=>
     {"id"=>2583,
      "name"=>"Incredible Cotton Car",
      "description"=>"Qui sint sed sint animi.",
      "owner_user_id"=>13938,
      "app_sponsor_id"=>345,
      "group_type"=>
       {"id"=>5185, "name"=>"Factory:Open", "description"=>"Open"},
      "owner"=>
       {"id"=>13938,
        "first_name"=>"Price",
        "last_name"=>"Marks",
        "title"=>"Creator Of All 1",
        "organization_name"=>"Keeling-Simonis",
        "photo"=>"www.example.com/user_photo.jpg",
        "user_role_id"=>29992,
        "user_connection_id"=>nil}},
    "user"=>
     {"id"=>13935,
      "first_name"=>"Jazmyn",
      "last_name"=>"Bahringer",
      "title"=>"Author",
      "organization_name"=>"Lubowitz-Rosenbaum",
      "photo"=>"www.example.com/user_photo.jpg",
      "user_role_id"=>29987,
      "user_connection_id"=>nil}},
   {"id"=>1057,
    "title"=>
     "Polarised leading edge artificial intelligence: Ergonomic Granite Shirt",
    "body"=>
     "---\n- Earum ea voluptates qui assumenda. Deleniti fugiat est. Facere omnis reprehenderit\n  et provident ad
    "body_markdown"=>
     "---\n- Reiciendis in id dolorem distinctio qui ut vel. Est rerum beatae pariatur. Ab et\n  ea. Aut eos volup
    "excerpt"=>"Reverse-engineered user-facing product",
    "thumbnail_teaser_photo"=>"www.example.com/post_thumbnail.jpg",
    "display_rank"=>1,
    "view_count"=>2,
    "created_by"=>nil,
    "updated_by"=>nil,
    "group"=>
     {"id"=>2584,
      "name"=>"Sleek Rubber Shoes",
      "description"=>"Ipsum aut nam velit sint sint velit alias.",
      "owner_user_id"=>13941,
      "app_sponsor_id"=>346,
      "group_type"=>
       {"id"=>5186, "name"=>"Factory:Open", "description"=>"Open"},
      "owner"=>
       {"id"=>13941,
        "first_name"=>"Josefina",
        "last_name"=>"Powlowski",
        "title"=>"Creator Of All 1",
        "organization_name"=>"Blick Group",
        "photo"=>"www.example.com/user_photo.jpg",
        "user_role_id"=>29995,
        "user_connection_id"=>nil}},
    "user"=>
     {"id"=>13935,
      "first_name"=>"Jazmyn",
      "last_name"=>"Bahringer",
      "title"=>"Author",
      "organization_name"=>"Lubowitz-Rosenbaum",
      "photo"=>"www.example.com/user_photo.jpg",
      "user_role_id"=>29987,
      "user_connection_id"=>nil}}]}
```

This requests provides a <strong>HTML 200</strong> on success.