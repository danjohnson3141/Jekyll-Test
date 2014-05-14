<!-- --- title: GET /post_likes/users/:post_id -->

Returns **all** post likes for **one** post.

=
#### Authentication

The user needs to be logged in and have valid credentials to use this route.

=
#### Parameters

:post_id - Integer, passed in through the URL. Is derived from the 'id' field on the 'posts' table.

=
####API request example:
```json
http://stage-api-access.evant.com/post_likes/user/2304
```

=
####JSON response example:

```json
{"post_likes"=>
  [{"id"=>708,
    "post_id"=>2304,
    "ago"=>"0m",
    "user"=>
     {"id"=>32788,
      "first_name"=>"Generic",
      "last_name"=>"User",
      "user_connection_id"=>nil}},
   {"id"=>709,
    "post_id"=>2304,
    "ago"=>"0m",
    "user"=>
     {"id"=>32793,
      "first_name"=>"Stefan",
      "last_name"=>"Berge",
      "user_connection_id"=>nil}},
   {"id"=>710,
    "post_id"=>2304,
    "ago"=>"0m",
    "user"=>
     {"id"=>32794,
      "first_name"=>"Cecile",
      "last_name"=>"Spinka",
      "user_connection_id"=>nil}},
   {"id"=>711,
    "post_id"=>2304,
    "ago"=>"0m",
    "user"=>
     {"id"=>32795,
      "first_name"=>"Donato",
      "last_name"=>"Schimmel",
      "user_connection_id"=>nil}},
   {"id"=>712,
    "post_id"=>2304,
    "ago"=>"0m",
    "user"=>
     {"id"=>32796,
      "first_name"=>"Derick",
      "last_name"=>"Abshire",
      "user_connection_id"=>nil}},
   {"id"=>713,
    "post_id"=>2304,
    "ago"=>"0m",
    "user"=>
     {"id"=>32797,
      "first_name"=>"Robbie",
      "last_name"=>"Rogahn",
      "user_connection_id"=>nil}}]}
```

This requests provides a <strong>HTML 200</strong> on success.