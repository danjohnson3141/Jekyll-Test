<!-- --- title: GET /post_comments/:id -->

Returns **one** post comment.

=
#### Authentication

The user needs to be logged in and have valid credentials to use this route.

=
#### Parameters

(post_comments) :id - Integer, passed in the URL. Is derived from the 'id' field on the 'post_comments' table.

=
####JSON request example:
```json
http://0.0.0.0:3000/post_comments/148
```

=
####JSON response example:

```json
{"post_comment"=>
  {"id"=>148,
   "body"=>"Ameliorated neutral productivity",
   "user"=>
    {"id"=>38128,
     "email"=>"mattie.fay@faheyconsidine.info",
     "alt_email"=>"beatrice@hotmail.com",
     "first_name"=>"Nikko",
     "last_name"=>"Beatty",
     "title"=>"Author",
     "organization_name"=>"Welch-Mills",
     "bio"=>
      "Deserunt molestias perspiciatis autem esse voluptas qui enim facilis aut dolorum fuga vitae magni.",
     "photo"=>
      "https://assets.evanta.com/shared/resources/Users/large/anonymous2.jpg",
     "can_message"=>true,
     "user_role_id"=>37765,
     "user_connection_id"=>nil,
     "post_count"=>0},
   "post"=>
    {"id"=>3499,
     "title"=>"Total intangible support: Fantastic Rubber Shoes",
     "excerpt"=>"Ameliorated secondary concept",
     "body"=>
      "---\n- Ut explicabo sunt. Sed ad optio tenetur vitae quasi aut vel. Voluptatem dicta porro.\n- Modi qui et culpa dolores et. Ad dolore nostrum. Commodi accusantium enim odit est\n  amet ipsam fugiat.\n- Illum minus ducimus est placeat eveniet. Animi ullam quidem. Ut molestiae et labore.\n  Voluptas consectetur maiores rerum possimus qui aut id.\n- Odio voluptates voluptatem eius ut est. Consectetur dolores minus quae ut deleniti\n  aut corporis. Ut nihil deserunt rem maxime molestiae. Autem ab voluptatem et reiciendis.\n  Laboriosam non veniam ut dolores in et.\n- At placeat doloribus. Molestiae doloremque quia quidem beatae maiores. Mollitia\n  quo porro impedit beatae rerum vitae sit. Aspernatur voluptatibus voluptas modi\n  recusandae animi magni aut.\n",
     "body_markdown"=>
      "---\n- Itaque sit quo eum autem suscipit. Sunt aut laudantium voluptas sed. Temporibus\n  quisquam quibusdam et ut.\n- Quis quia architecto odio reprehenderit soluta numquam. Nostrum harum doloribus\n  distinctio ipsum. Non maiores aut ullam quas occaecati omnis. Qui magnam natus labore\n  magni in sapiente.\n- Voluptatem iste consequatur id voluptas et fugit voluptatem. Voluptatem earum sint\n  asperiores vitae doloremque minima. Placeat et esse. Tempore voluptatum veritatis\n  suscipit at. Quasi in tempore sit maxime.\n- Tenetur molestiae qui perspiciatis inventore perferendis. Asperiores nobis est blanditiis.\n  Reprehenderit recusandae mollitia cum.\n- Voluptatem ea eum eaque nulla eum tenetur. Sapiente magni inventore vero et quia\n  iste. Quam ratione impedit fugiat excepturi vero eos nihil. Dolorem vel maiores\n  ipsum numquam.\n",
     "thumbnail_teaser_photo"=>"www.example.com/post_thumbnail.jpg",
     "display_rank"=>0,
     "view_count"=>0,
     "like_count"=>0,
     "comment_count"=>0,
     "post_like_id"=>nil,
     "post_attachments"=>[],
     "ago"=>"0m",
     "group"=>nil,
     "event"=>{"id"=>6653, "name"=>"Fantastic Wooden Pants 362"},
     "authors"=>[nil]}}}
[2] pry(#<RSpec::ExampleG
```

This requests provides a <strong>HTML 200</strong> on success.