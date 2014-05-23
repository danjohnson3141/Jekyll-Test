<!-- --- title: GET /featured_posts/event/:event_id -->

Featured posts are a list of posts that the application displays at the top of several pages (currently: user feed, group feed, event feed). There is no maximum number of posts that will be returned by this route. However, it is possible to artificially limit the number of posts returned through a suffix on the route, which is: '?limit=X' where X is the number to return.

The database table that manages this route only has two relevant fields that are addressed by the application, they are 'post_id' and 'created_at'. The post_id is just the reference to the post that should appear in the feed, created_at is only relevant for purposes of sorting the list.

This particular route returns all of the featured posts that reference the event_id passed in.

=
####Authentication:

The user needs to be logged in and have valid credentials to use this route.

=
####Parameters:

:event_id - Integer, passed in through the URL. Is derived from the 'event_id' field on the 'event_featured_posts' table.

=
####API request example:
```html
http://stage-api-access.evant.com/featured_posts/event/4316
```

=
####JSON response example:

```json
{"event_featured_posts"=>
  [{"id"=>258,
    "event_id"=>4316,
    "post"=>
     {"id"=>1223,
      "title"=>"Implemented next generation neural-net: Rustic Steel Shoes",
      "body"=>
       "---\n- Aspernatur laboriosam quis. Neque et aut dolores doloribus facilis qui vel. Molestias\n  et molesti
      "body_markdown"=>
       "---\n- Ipsam et est. Eum expedita iste enim. Soluta facere quaerat est. Magnam maxime tenetur\n  sunt mole
      "excerpt"=>"Horizontal regional model",
      "thumbnail_teaser_photo"=>"www.example.com/post_thumbnail.jpg",
      "display_rank"=>0,
      "view_count"=>1,
      "show_likes_count"=>false,
      "like_count"=>0,
      "post_likeable"=>false,
      "view_post_likes_list"=>false,
      "post_attachments"=>[],
      "user"=>
       {"id"=>33457,
        "first_name"=>"Quinn",
        "last_name"=>"Predovic",
        "title"=>"Random User",
        "organization_name"=>"Boehm, Effertz and Stark",
        "photo"=>
         "https://assets.evanta.com/shared/resources/Users/large/anonymous2.jpg",
        "user_role_id"=>33459}}},
   {"id"=>259,
    "event_id"=>4316,
    "post"=>
     {"id"=>1224,
      "title"=>
       "Open-source solution-oriented encryption: Intelligent Steel Pants",
      "body"=>
       "---\n- Qui hic eos. Commodi debitis assumenda a. Quia veritatis quo ut et assumenda. Eius\n  laudantium ve
      "body_markdown"=>
       "---\n- Nisi eligendi tenetur nesciunt pariatur consequatur. Doloremque repudiandae consectetur\n  cumque d
      "excerpt"=>"Vision-oriented foreground utilisation",
      "thumbnail_teaser_photo"=>"www.example.com/post_thumbnail.jpg",
      "display_rank"=>0,
      "view_count"=>0,
      "show_likes_count"=>false,
      "like_count"=>0,
      "post_likeable"=>false,
      "view_post_likes_list"=>false,
      "post_attachments"=>[],
      "user"=>
       {"id"=>33463,
        "first_name"=>"Marcelle",
        "last_name"=>"Runolfsson",
        "title"=>"Random User",
        "organization_name"=>"Reichert, Reinger and Stracke",
        "photo"=>
         "https://assets.evanta.com/shared/resources/Users/large/anonymous2.jpg",
        "user_role_id"=>33465}}},
   {"id"=>260,
    "event_id"=>4316,
    "post"=>
     {"id"=>1225,
      "title"=>"Vision-oriented system-worthy benchmark: Practical Wooden Hat",
      "body"=>
       "---\n- Officia pariatur in distinctio et dignissimos ea quibusdam. Numquam et vel consequatur.\n  Assumend
      "body_markdown"=>
       "---\n- Voluptates sunt nemo et optio qui exercitationem. Laborum minima et. Ratione fuga\n  quam beatae qu
      "excerpt"=>"Right-sized actuating utilisation",
      "thumbnail_teaser_photo"=>"www.example.com/post_thumbnail.jpg",
      "display_rank"=>6,
      "view_count"=>7,
      "show_likes_count"=>false,
      "like_count"=>0,
      "post_likeable"=>false,
      "view_post_likes_list"=>false,
      "post_attachments"=>[],
      "user"=>
       {"id"=>33469,
        "first_name"=>"Madelynn",
        "last_name"=>"Dietrich",
        "title"=>"Random User",
        "organization_name"=>"Murazik, Wintheiser and Kiehn",
        "photo"=>
         "https://assets.evanta.com/shared/resources/Users/large/anonymous2.jpg",
        "user_role_id"=>33471}}}]}
```

This requests provides a <strong>HTML 200</strong> on success.