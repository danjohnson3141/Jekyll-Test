<!-- --- title: POST /post_likes -->

This is the method by which the active user is able to add a 'like' to any post.

=
####Authentication:

The user needs to be logged in and have valid credentials to use this route.

=
####Parameters:

:post_id - Integer, passed in through the post data. Is derived from the 'id' field on the 'post' table.

=
####API request example:
```html
http://example.com/post_like
```

=
###Post Data:
```json
{ post_like: { post_id: 1273 } }
```

=
####JSON response example:

```json
{"post_like"=>
  {"id"=>447,
   "ago"=>"0m",
   "user"=>
    {"id"=>17032,
     "first_name"=>"Generic",
     "last_name"=>"User",
     "user_connection_id"=>nil},
   "post"=>
    {"id"=>1273,
     "title"=>"Decentralized optimizing focus group: Small Wooden Gloves",
     "excerpt"=>"Upgradable analyzing secured line",
     "group"=>nil,
     "event"=>{"id"=>2717, "name"=>"Sleek Plastic Pants 3"}}}}
```

This requests provides a <strong>HTML 201</strong> on success.