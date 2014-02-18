This returns **one** post.

=
#### Authentication

The user needs to be logged in and have valid credentials to use this route.

=
#### Parameters

:post_id

This is derived from the 'id' field on 'posts' table.

=
####JSON request example:
```
http://0.0.0.0:3000/posts/21
```

=
####JSON response example:

```
{"post"=>
  {"id"=>21,
   "title"=>"Profit-focused zero tolerance alliance: Sleek Steel Car",
   "body"=>
    "---\n- Aut illum sit dolorem dolor quo quia. Et aliquam alias voluptas provident iure placeat\n  magni. Et incidunt velit. Iure non et quas velit illum hic nemo. Vero debitis minima\n  autem.\n- Atque illo aut eos. Vero laboriosam ut quam aliquid eaque quisquam quasi. Molestiae\n  non voluptate quidem.\n- Nisi rerum laborum sit natus. Aperiam ut quos. Magnam nobis neque odio sint eaque.\n  Quia in sunt eum distinctio.\n- Eius velit iste sit voluptas ea enim impedit. Exercitationem sit velit sunt. Id\n  et quibusdam omnis voluptas. Quia omnis et. Accusamus sit minima et est.\n- Aut inventore ut tempora. Omnis consequatur dignissimos ad inventore rerum sed sequi.\n  Consequatur sequi earum. Voluptatem est ut asperiores nisi quibusdam ducimus quae.\n",
   "body_markdown"=>
    "---\n- Voluptatem eius perferendis aliquam illo quidem. Non enim dolores sint possimus\n  numquam suscipit sit. Qui totam voluptatibus velit dolores.\n- Reprehenderit ea sed eos. Sit at nam suscipit necessitatibus. Asperiores atque odio\n  eveniet quos adipisci dicta. Id blanditiis aperiam quo ut nostrum reprehenderit.\n- Recusandae at qui et est atque. Velit excepturi consectetur non ut non quaerat aspernatur.\n  Non facere nihil.\n- Vitae voluptatem et et voluptatum vel. Ipsam ea unde ut totam et. Nulla est est\n  distinctio eveniet molestiae perspiciatis. Nostrum ipsa corporis. Tenetur voluptates\n  est.\n- Saepe vel ea voluptatem sapiente. Architecto molestiae fugit porro nulla illum magni.\n  Asperiores quos exercitationem. Et et repudiandae distinctio perspiciatis ratione.\n",
   "excerpt"=>"Operative hybrid focus group",
   "thumbnail_teaser_photo"=>"www.example.com/post_thumbnail.jpg",
   "display_rank"=>0,
   "view_count"=>3,
   "group"=>
    {"id"=>108,
     "name"=>"Fantastic Plastic Gloves",
     "group_type_name"=>"Factory:Open"},
   "user"=>
    {"id"=>978,
     "first_name"=>"Aryanna",
     "last_name"=>"Senger",
     "title"=>"Author",
     "organization_name"=>"Ankunding, Bins and Renner",
     "photo"=>
      "https://assets.evanta.com/shared/resources/Users/large/anonymous.jpg",
     "user_role_id"=>980,
     "user_connection_id"=>nil}}}
```

This requests provides a <strong>HTML 200</strong> on success.