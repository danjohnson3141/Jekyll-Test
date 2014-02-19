This route returns the featured posts for **one** group.

=
#### Authentication

The user needs to be logged in and have valid credentials to use this route.

=
#### Parameters

:group_id - Integer, passed in through the URL. Is derived from the 'id' field on the 'groups' table.

=
####JSON request example:
```
http://0.0.0.0:3000//group_featured_posts/764
```

=
####JSON response example:

```
{"group_featured_posts"=>
  [{"id"=>31,
    "group_id"=>764,
    "post"=>
     {"id"=>218,
      "title"=>
       "Business-focused non-volatile initiative: Ergonomic Granite Pants",
      "body"=>
       "---\n- Veniam rerum et quam eveniet sit voluptas. Et laudantium ipsa neque aut fugit. Enim\n  eveniet deserunt vel. Non magni error cum dignissimos voluptatem.\n- Id autem voluptatem. Fugiat saepe repudiandae illo rerum adipisci ut amet. Eaque\n  sapiente illo.\n- Inventore et doloribus esse necessitatibus maxime voluptates. Non voluptate a et\n  temporibus excepturi nobis consectetur. Atque placeat eum omnis vitae.\n- Provident ullam eligendi. Dicta sit vel exercitationem. Nam est excepturi. Nesciunt\n  non quibusdam facilis. Omnis minima distinctio accusantium.\n- Ut dolorem eum perspiciatis. Iste dignissimos earum aut nihil quia. Quo eveniet\n  possimus sunt ullam illum voluptatibus omnis.\n",
      "body_markdown"=>
       "---\n- Magnam id ipsum sunt quo sed delectus eum. Minus ut eos consequuntur. Ea beatae\n  dignissimos.\n- Ducimus unde cum necessitatibus sed aperiam corporis error. Id sed beatae iusto\n  aspernatur autem nesciunt. Vel neque non ut.\n- Quasi a quidem. Minus iste maxime et. Et eum dolorem accusantium reprehenderit praesentium\n  aperiam nihil. Labore necessitatibus enim facere odio quis. Rerum perferendis maxime\n  est et.\n- Ad nam sequi nobis dolorem. Ut sit numquam aut aperiam quo repudiandae. Ducimus\n  quod non fugit eum.\n- Qui exercitationem provident. Eligendi non nostrum voluptatum nihil id dolore. Magnam\n  reiciendis dolorum ut. Fuga vitae eaque consequatur unde.\n",
      "excerpt"=>"Self-enabling context-sensitive data-warehouse",
      "thumbnail_teaser_photo"=>"www.example.com/post_thumbnail.jpg",
      "display_rank"=>5,
      "view_count"=>5,
      "user"=>
       {"id"=>6464,
        "first_name"=>"Una",
        "last_name"=>"Harber",
        "title"=>"Random User",
        "organization_name"=>"Stracke Inc",
        "photo"=>
         "https://assets.evanta.com/shared/resources/Users/large/anonymous.jpg",
        "user_role_id"=>6466,
        "user_connection_id"=>nil}}},
   {"id"=>32,
    "group_id"=>764,
    "post"=>
     {"id"=>219,
      "title"=>
       "Fundamental bandwidth-monitored flexibility: Rustic Steel Chair",
      "body"=>
       "---\n- Omnis voluptatem necessitatibus. Necessitatibus et architecto ad commodi error.\n  Sunt repudiandae nesciunt ut et voluptatibus qui.\n- Quaerat doloremque voluptas non eius. Minima omnis itaque beatae voluptas. Et ea\n  quam magnam.\n- Quia consectetur enim. Maiores ut nobis. Voluptas et architecto iste.\n- Consequuntur itaque voluptatibus in dolore pariatur doloremque. Nostrum totam sed\n  sapiente. Ut sed minima ipsam quibusdam voluptate et ea. Praesentium corrupti quibusdam\n  aspernatur non. Maiores libero ut culpa dignissimos tempore.\n- Numquam eum ab molestiae. Repellendus voluptatem voluptatem culpa. Excepturi esse\n  libero. Sunt dolorem nobis enim.\n",
      "body_markdown"=>
       "---\n- Modi ad eveniet quisquam assumenda explicabo sequi dignissimos. Rerum rerum vel.\n  Est provident molestias sit. Suscipit debitis aut culpa pariatur nihil.\n- Rerum cupiditate praesentium voluptatem cumque aperiam. Asperiores rerum distinctio\n  natus beatae enim. Atque nam soluta reiciendis debitis.\n- Beatae ea ea modi. Id culpa quis fuga incidunt hic numquam quia. Tenetur soluta\n  sequi placeat quis maiores.\n- Soluta id quas qui quo temporibus ea facere. Qui autem iste. Nam voluptas ut minima\n  culpa asperiores omnis sunt. Incidunt sit accusamus ut ullam voluptatem omnis quibusdam.\n  Voluptatem non ad possimus consequatur.\n- Optio et enim maiores. Qui dicta voluptatem consequuntur necessitatibus omnis ipsam\n  dolor. Amet voluptas in aliquam nihil ut voluptas.\n",
      "excerpt"=>"Configurable web-enabled definition",
      "thumbnail_teaser_photo"=>"www.example.com/post_thumbnail.jpg",
      "display_rank"=>3,
      "view_count"=>8,
      "user"=>
       {"id"=>6467,
        "first_name"=>"Dane",
        "last_name"=>"Hessel",
        "title"=>"Random User",
        "organization_name"=>"Nicolas Group",
        "photo"=>
         "https://assets.evanta.com/shared/resources/Users/large/anonymous.jpg",
        "user_role_id"=>6469,
        "user_connection_id"=>nil}}}]}
```

This requests provides a <strong>HTML 200</strong> on success.