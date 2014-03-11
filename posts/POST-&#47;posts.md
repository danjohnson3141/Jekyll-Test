<!-- --- title: POST /posts -->

This is the route by which users will create *new* posts.

=
#### Authentication

The user needs to be logged in and have valid credentials to use this route.

=
#### Parameters

:title - Text, passed in through the post data. The title of the post. Limited to 255 characters. 

:body - Text, passed in through the post data. The plain text of the post.

:body_markdown - Text, passed in through the post data. The formatted version of the post. 

:excerpt - Text, passed in through the post data. A synopsis of the post.

:thumbnail_teaser_photo - Varchar, passed in through the post data. The URL of a photo used to advertise the post

:group_id - Integer, passed in through the post data. This is the 'id' of the group that the post will be associated with; derived from the 'id' field on the 'groups' table.

=
####JSON request example:
```json
http://0.0.0.0:3000/posts
```

=
####JSON response example:

```json
{"post"=>
  {"id"=>81,
   "title"=>"Teapot",
   "body"=>"A teapot is a vessel used for steeping tea leaves.",
   "body_markdown"=>"A *teapot* is a vessel used for **steeping** tea leaves.",
   "excerpt"=>"vessel steeping",
   "thumbnail_teaser_photo"=>"www.example.com/teaser_photo.bmp",
   "display_rank"=>nil,
   "view_count"=>nil,
   "group"=>
    {"id"=>268,
     "name"=>"Intelligent Concrete Pants",
     "group_type_name"=>"Factory:Open"},
   "user"=>
    {"id"=>2228,
     "first_name"=>"Generic",
     "last_name"=>"User",
     "title"=>"CEO of QA",
     "organization_name"=>"Evanta",
     "photo"=>
      "https://assets.evanta.com/shared/resources/Users/large/anonymous.jpg",
     "user_role_id"=>2232,
     "user_connection_id"=>nil}}}
```

This requests provides a <strong>HTML 201</strong> on success.