<!-- --- title: GET /post_comments/post/:post_id -->

Returns **all** comments associated with **one** post.

=
####Authentication:

The user needs to be logged in and have valid credentials to use this route.

=
####Parameters:

(post) :id - Integer, passed in through the URL. Is derived from the 'id' field on the 'posts' table.

=
####API request example:
```html
http://stage-api-access.evant.com/post_comments/post/3758
```

=
####JSON response example:

```json
"post_comments"=>
  [{"id"=>159,
    "body"=>"Ameliorated tertiary policy",
    "user"=>
     {"id"=>40471,
      "email"=>"generic_user@evanta.com",
      "alt_email"=>"alt_gen_use@evanta.com",
      "first_name"=>"Generic",
      "last_name"=>"User",
      "title"=>"CEO of QA",
      "organization_name"=>"Evanta",
      "bio"=>"This is the biography of the default Generic User",
      "photo"=>
       "https://assets.evanta.com/shared/resources/Users/large/anonymous2.jpg",
      "can_message"=>true,
      "user_role_id"=>40108,
      "user_connection_id"=>nil,
      "post_count"=>1},
    "post"=>
     {"id"=>3758,
      "title"=>"Reactive homogeneous encryption: Incredible Cotton Shirt",
      "excerpt"=>"Integrated optimal concept",
      "body"=>
       "---\n- Qui et voluptatum. Repellendus omnis laborum. Totam ipsum minus quia autem voluptatem\n  provident 
      "body_markdown"=>
       "---\n- Neque est nulla nostrum omnis corrupti fuga qui. Id sint eveniet sequi fuga eum\n  sed. Voluptatem 
      "thumbnail_teaser_photo"=>"www.example.com/post_thumbnail.jpg",
      "display_rank"=>0,
      "view_count"=>5,
      "like_count"=>0,
      "comment_count"=>0,
      "post_like_id"=>nil,
      "post_attachments"=>[],
      "ago"=>"0m",
      "group"=>nil,
      "event"=>{"id"=>7150, "name"=>"Gorgeous Granite Shoes 265"},
      "authors"=>
       [{"id"=>40471,
         "first_name"=>"Generic",
         "last_name"=>"User",
         "title"=>"CEO of QA",
         "organization_name"=>"Evanta",
         "photo"=>
          "https://assets.evanta.com/shared/resources/Users/large/anonymous2.jpg"}]}},
   {"id"=>160,
    "body"=>"Exclusive fault-tolerant info-mediaries",
    "user"=>
     {"id"=>40472,
      "email"=>"augusta.kiehn@rogahn.name",
      "alt_email"=>"jensen@hotmail.com",
      "first_name"=>"Katrina",
      "last_name"=>"Gorczany",
      "title"=>"Author",
      "organization_name"=>"Stokes, Hilpert and Kertzmann",
      "bio"=>
       "Eaque sit beatae harum corporis autem tempore error dolore distinctio atque ex est est nesciunt.",
      "photo"=>
       "https://assets.evanta.com/shared/resources/Users/large/anonymous2.jpg",
      "can_message"=>true,
      "user_role_id"=>40109,
      "user_connection_id"=>nil,
      "post_count"=>0},
    "post"=>
     {"id"=>3758,
      "title"=>"Reactive homogeneous encryption: Incredible Cotton Shirt",
      "excerpt"=>"Integrated optimal concept",
      "body"=>
       "---\n- Qui et voluptatum. Repellendus omnis laborum. Totam ipsum minus quia autem voluptatem\n  provident 
      "body_markdown"=>
       "---\n- Neque est nulla nostrum omnis corrupti fuga qui. Id sint eveniet sequi fuga eum\n  sed. Voluptatem 
      "thumbnail_teaser_photo"=>"www.example.com/post_thumbnail.jpg",
      "display_rank"=>0,
      "view_count"=>5,
      "like_count"=>0,
      "comment_count"=>0,
      "post_like_id"=>nil,
      "post_attachments"=>[],
      "ago"=>"0m",
      "group"=>nil,
      "event"=>{"id"=>7150, "name"=>"Gorgeous Granite Shoes 265"},
      "authors"=>
       [{"id"=>40471,
         "first_name"=>"Generic",
         "last_name"=>"User",
         "title"=>"CEO of QA",
         "organization_name"=>"Evanta",
         "photo"=>
          "https://assets.evanta.com/shared/resources/Users/large/anonymous2.jpg"}]}}]}
```

This requests provides a <strong>HTML 200</strong> on success.