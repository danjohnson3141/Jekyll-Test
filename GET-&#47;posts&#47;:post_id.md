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
http://0.0.0.0:3000/posts/921
```

=
####JSON response example:

```
{"post"=>
  {"id"=>921,
   "title"=>"Operative modular conglomeration: Practical Plastic Computer",
   "body"=>
    "---\n- Blanditiis quia ab nemo asperiores et ea quia. Porro in laboriosam mollitia eum.\n  Eum perferendis ma
   "body_markdown"=>
    "---\n- Nihil autem et est. At ducimus sit et eum. Id eligendi autem ut. Et molestiae consectetur\n  distincti
   "excerpt"=>"Optimized assymetric algorithm",
   "thumbnail_teaser_photo"=>"www.example.com/post_thumbnail.jpg",
   "display_rank"=>0,
   "view_count"=>7,
   "created_by"=>
    {"id"=>10606,
     "email"=>"carolina_becker@baileyeffertz.biz",
     "created_at"=>"2014-02-18T17:01:57.000Z",
     "updated_at"=>"2014-02-18T17:01:57.000Z",
     "alt_email"=>"jon_okuneva@hotmail.com",
     "first_name"=>"Jadyn",
     "last_name"=>"Hackett",
     "title"=>"Author",
     "organization_name"=>"Moen and Sons",
     "bio"=>
      "Rerum similique saepe architecto tenetur velit dolores aut quia omnis quos dolorum cupiditate harum odit.",
     "app_language_id"=>1,
     "photo"=>"www.example.com/user_photo.jpg",
     "user_role_id"=>26658,
     "created_by"=>
      {"id"=>10604,
       "email"=>"norbert@gleichner.net",
       "created_at"=>"2014-02-18T17:01:57.000Z",
       "updated_at"=>"2014-02-18T17:01:57.000Z",
       "alt_email"=>"hank.botsford@yahoo.com",
       "first_name"=>"Mozelle",
       "last_name"=>"Mraz",
       "title"=>"Creator Of All 1",
       "organization_name"=>"Batz-Farrell",
       "bio"=>
        "Optio error est id molestiae sed ratione unde explicabo laudantium autem sapiente.",
       "app_language_id"=>1,
       "photo"=>"www.example.com/user_photo.jpg",
       "user_role_id"=>26659,
       "created_by"=>nil,
       "updated_by"=>nil},
     "updated_by"=>
      {"id"=>10605,
       "email"=>"nicklaus@johns.biz",
       "created_at"=>"2014-02-18T17:01:57.000Z",
       "updated_at"=>"2014-02-18T17:01:57.000Z",
       "alt_email"=>"kianna.crona@yahoo.com",
       "first_name"=>"Henri",
       "last_name"=>"Ledner",
       "title"=>"Creator Of All 1",
       "organization_name"=>"Hodkiewicz-Schroeder",
       "bio"=>
        "Animi eos qui labore voluptatum velit illum repellendus qui incidunt nemo sed nobis eos.",
       "app_language_id"=>1,
       "photo"=>"www.example.com/user_photo.jpg",
       "user_role_id"=>26660,
       "created_by"=>nil,
       "updated_by"=>nil}},
   "updated_by"=>
    {"id"=>10606,
     "email"=>"carolina_becker@baileyeffertz.biz",
     "created_at"=>"2014-02-18T17:01:57.000Z",
     "updated_at"=>"2014-02-18T17:01:57.000Z",
     "alt_email"=>"jon_okuneva@hotmail.com",
     "first_name"=>"Jadyn",
     "last_name"=>"Hackett",
     "title"=>"Author",
     "organization_name"=>"Moen and Sons",
     "bio"=>
      "Rerum similique saepe architecto tenetur velit dolores aut quia omnis quos dolorum cupiditate harum odit.",
     "app_language_id"=>1,
     "photo"=>"www.example.com/user_photo.jpg",
     "user_role_id"=>26658,
     "created_by"=>
      {"id"=>10604,
       "email"=>"norbert@gleichner.net",
       "created_at"=>"2014-02-18T17:01:57.000Z",
       "updated_at"=>"2014-02-18T17:01:57.000Z",
       "alt_email"=>"hank.botsford@yahoo.com",
       "first_name"=>"Mozelle",
       "last_name"=>"Mraz",
       "title"=>"Creator Of All 1",
       "organization_name"=>"Batz-Farrell",
       "bio"=>
        "Optio error est id molestiae sed ratione unde explicabo laudantium autem sapiente.",
       "app_language_id"=>1,
       "photo"=>"www.example.com/user_photo.jpg",
       "user_role_id"=>26659,
       "created_by"=>nil,
       "updated_by"=>nil},
     "updated_by"=>
      {"id"=>10605,
       "email"=>"nicklaus@johns.biz",
       "created_at"=>"2014-02-18T17:01:57.000Z",
       "updated_at"=>"2014-02-18T17:01:57.000Z",
       "alt_email"=>"kianna.crona@yahoo.com",
       "first_name"=>"Henri",
       "last_name"=>"Ledner",
       "title"=>"Creator Of All 1",
       "organization_name"=>"Hodkiewicz-Schroeder",
       "bio"=>
        "Animi eos qui labore voluptatum velit illum repellendus qui incidunt nemo sed nobis eos.",
       "app_language_id"=>1,
       "photo"=>"www.example.com/user_photo.jpg",
       "user_role_id"=>26660,
       "created_by"=>nil,
       "updated_by"=>nil}},
   "group"=>
    {"id"=>2178,
     "name"=>"Awesome Cotton Chair",
     "description"=>
      "Eum occaecati molestias veritatis est recusandae sapiente et quos explicabo.",
     "owner_user_id"=>10609,
     "app_sponsor_id"=>132,
     "group_type"=>{"id"=>4444, "name"=>"Factory:Open", "description"=>"Open"},
     "owner"=>
      {"id"=>10609,
       "first_name"=>"Luciano",
       "last_name"=>"Wilkinson",
       "title"=>"Creator Of All 1",
       "organization_name"=>"White Inc",
       "photo"=>"www.example.com/user_photo.jpg",
       "user_role_id"=>26663,
       "user_connection_id"=>nil}},
   "user"=>
    {"id"=>10606,
     "first_name"=>"Jadyn",
     "last_name"=>"Hackett",
     "title"=>"Author",
     "organization_name"=>"Moen and Sons",
     "photo"=>"www.example.com/user_photo.jpg",
     "user_role_id"=>26658,
     "user_connection_id"=>nil}}}
```

This requests provides a <strong>HTML 200</strong> on success.