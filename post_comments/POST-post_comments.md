<!-- --- title: POST /post_comments -->

This the method by which the active user ads a comment to an already existing post.

=
#### Authentication

The user needs to be logged in and have valid credentials to use this route.

=
#### Parameters

:body - Text, passed in through the post data. This is the plain text of the submission.
:post_id - Integer, passed in through the post data. Is derived from the 'id' field on the 'post' table.


=
####JSON request example:
```json
http://stage-api-access.evant.com/post_comments
```

=
###Post Data:
```json
{ post_comment: { body: 'Awesome post dude!', post_id: 1053 } }
```

=
####JSON response example:

```json
{"post_comment"=>
  {"id"=>87,
   "body"=>"Awesome post dude!",
   "user"=>
    {"id"=>14083,
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
     "user_role_id"=>18425,
     "user_connection_id"=>nil,
     "post_count"=>1,
     "post_like_count"=>0,
     "post_comment_count"=>1,
     "user_connection_count"=>0},
   "post"=>
    {"id"=>1053,
     "title"=>"Ameliorated hybrid concept: Small Wooden Hat",
     "post_excerpt"=>"Polarised tertiary workforce",
     "body"=>
      "---\n- Et est qui rerum earum quis. Consequatur in nesciunt nisi consectetur. Aliquid nobis\n  voluptas repellendus unde laudantium quis nam.\n- Est aspernatur consequatur. Vel aut deserunt enim. Consequatur architecto temporibus\n  mollitia at. Aut labore facere mollitia qui odio veritatis. Consequatur omnis ut\n  harum.\n- Ducimus esse omnis perspiciatis qui iusto sit. Aut ut unde aperiam consequatur modi.\n  Deleniti pariatur voluptatem eveniet. Alias omnis provident tenetur ea omnis fugiat.\n  Architecto quo est eum non voluptatem voluptatem.\n- Est aut maiores dolor. Et rerum doloremque exercitationem voluptates. Velit eaque\n  quas velit sapiente enim ut eos. Voluptas nam aspernatur ratione id veritatis.\n- Aspernatur consequatur ut quaerat. Nisi voluptatem consequatur officia beatae voluptatem\n  qui fugit. Dolores mollitia commodi ea. Velit quam a odit esse doloribus sit exercitationem.\n  Voluptate quidem molestiae ab ex placeat voluptatum.\n",
     "body_markdown"=>
      "---\n- In recusandae quisquam dolorem non excepturi. Aliquid et voluptatibus. Totam ipsa\n  nesciunt ab aliquid numquam.\n- Nemo libero natus ab qui sit laboriosam voluptatibus. Ut voluptas facere nesciunt\n  non praesentium quae ad. Non voluptatibus fuga tempora molestiae distinctio tempore.\n- Sed iste accusamus ut veritatis. Commodi quia quibusdam repellat dolores. Consequatur\n  hic sit et pariatur voluptatibus velit dolorum.\n- Sint repellat sit exercitationem illo modi qui et. Sit et aperiam. Sit est ex.\n- Omnis dolorum eum ea facilis officiis placeat. Excepturi ducimus velit consectetur\n  amet est sit. Nobis perferendis magni consectetur aspernatur similique et. Et consequatur\n  in quibusdam.\n",
     "thumbnail_teaser_photo"=>"www.example.com/post_thumbnail.jpg",
     "display_rank"=>7,
     "view_count"=>7,
     "like_count"=>0,
     "comment_count"=>1,
     "post_like_id"=>nil,
     "post_attachments"=>[],
     "ago"=>"0m",
     "group"=>nil,
     "event"=>{"id"=>2225, "name"=>"Intelligent Steel Pants 53"},
     "sponsor"=>nil,
     "authors"=>
      [{"id"=>14083,
        "first_name"=>"Generic",
        "last_name"=>"User",
        "title"=>"CEO of QA",
        "organization_name"=>"Evanta",
        "photo"=>
         "https://assets.evanta.com/shared/resources/Users/large/anonymous2.jpg"}]}}}
```

This requests provides a <strong>HTML 201</strong> on success.