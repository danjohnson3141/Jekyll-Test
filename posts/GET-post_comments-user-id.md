<!-- --- title: GET /post_comments/user/:user_id -->

Returns **all** of the post comments for **one** user. 

=
#### Authentication

The user needs to be logged in and have valid credentials to use this route.

=
#### Parameters

:user_id - Integer, passed in through the URL. Is derived from the 'id' field on the 'users' table.

=
####JSON request example:
```json
http://0.0.0.0:3000/post_comments/user/19429
```

=
####JSON response example:

```json
{"post_comments"=>
  [{"id"=>96,
    "body"=>"Reverse-engineered reciprocal hub",
    "user"=>
     {"id"=>19429,
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
      "user_role_id"=>19198,
      "user_connection_id"=>nil,
      "post_count"=>1,
      "post_like_count"=>0,
      "post_comment_count"=>2,
      "user_connection_count"=>0},
    "post"=>
     {"id"=>1364,
      "title"=>"User-centric high-level application: Small Plastic Gloves",
      "excerpt"=>"Universal analyzing algorithm",
      "body"=>
       "---\n- Magnam aperiam ducimus ullam. Qui ut atque omnis. Sequi repellat consequatur eaque\n  dolores eos a
      "body_markdown"=>
       "---\n- Autem iusto sit aut. Doloribus repellat sed nisi commodi tempora dolorem. Repellat\n  eius mollitia
      "thumbnail_teaser_photo"=>"www.example.com/post_thumbnail.jpg",
      "display_rank"=>3,
      "view_count"=>0,
      "like_count"=>0,
      "comment_count"=>1,
      "post_like_id"=>nil,
      "post_attachments"=>[],
      "ago"=>"0m",
      "group"=>nil,
      "event"=>{"id"=>3078, "name"=>"Rustic Cotton Shoes 153"},
      "authors"=>[nil]}},
   {"id"=>97,
    "body"=>"Adaptive incremental groupware",
    "user"=>
     {"id"=>19429,
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
      "user_role_id"=>19198,
      "user_connection_id"=>nil,
      "post_count"=>1,
      "post_like_count"=>0,
      "post_comment_count"=>2,
      "user_connection_count"=>0},
    "post"=>
     {"id"=>1365,
      "title"=>"Customizable secondary monitoring: Gorgeous Plastic Shirt",
      "excerpt"=>"Self-enabling systemic algorithm",
      "body"=>
       "---\n- Occaecati recusandae enim eum reprehenderit velit voluptatem voluptates. Ab odit\n  reiciendis cons
      "body_markdown"=>
       "---\n- Itaque nostrum quod est placeat. Odio maiores modi cumque consequatur in esse qui.\n  Omnis officia
      "thumbnail_teaser_photo"=>"www.example.com/post_thumbnail.jpg",
      "display_rank"=>7,
      "view_count"=>4,
      "like_count"=>0,
      "comment_count"=>1,
      "post_like_id"=>nil,
      "post_attachments"=>[],
      "ago"=>"0m",
      "group"=>nil,
      "event"=>{"id"=>3079, "name"=>"Fantastic Steel Gloves 154"},
      "authors"=>[nil]}}]}
```

This requests provides a <strong>HTML 200</strong> on success.