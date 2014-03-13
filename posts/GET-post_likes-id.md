<!-- --- title: GET /post_likes/:id -->

Returns **one** post like based off the id passed in.

=
#### Authentication

The user needs to be logged in and have valid credentials to use this route.

=
#### Parameters

(post likes) :id - Integer, passed in through the URL. Is derived from the 'id' field on the 'post_likes' table.

=
####JSON request example:
```json
http://0.0.0.0:3000/post_likes/553
```

=
####JSON response example:

```json
{"post_like"=>
  {"id"=>533,
   "ago"=>"0m",
   "user"=>
    {"id"=>23337,
     "first_name"=>"Elvis",
     "last_name"=>"McDermott",
     "user_connection_id"=>nil},
   "post"=>
    {"id"=>1660,
     "title"=>"Customizable discrete flexibility: Gorgeous Steel Pants",
     "excerpt"=>"Fully-configurable multimedia array",
     "group"=>nil,
     "event"=>{"id"=>3640, "name"=>"Rustic Rubber Chair 220"}}}}
```

This requests provides a <strong>HTML 200</strong> on success.