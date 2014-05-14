<!-- --- title: GET /post_likes/posts/:user_id -->

Retuns **all** of the post likes for **one** users.

=
#### Authentication

The user needs to be logged in and have valid credentials to use this route.

=
#### Parameters

:user_id - Integer, passed in through the URL. Is derived from the 'id' field on the 'users' table.

=
####API request example:
```json
http://stage-api-access.evant.com/post_likes/posts/27461
```

=
####JSON response example:

```json
{"post_likes"=>
  [{"id"=>597,
    "user_id"=>27461,
    "ago"=>"1m",
    "post"=>
     {"id"=>1914,
      "title"=>
       "Reverse-engineered assymetric standardization: Small Steel Shoes",
      "excerpt"=>"Digitized web-enabled methodology",
      "group"=>
       {"id"=>6662,
        "name"=>"Small Rubber Hat 82",
        "group_type_name"=>"Factory:Open"},
      "event"=>nil}},
   {"id"=>599,
    "user_id"=>27461,
    "ago"=>"4m",
    "post"=>
     {"id"=>1916,
      "title"=>"Implemented demand-driven methodology: Awesome Steel Shirt",
      "excerpt"=>"Visionary context-sensitive website",
      "group"=>
       {"id"=>6664,
        "name"=>"Rustic Steel Shirt 83",
        "group_type_name"=>"Factory:Open"},
      "event"=>nil}},
   {"id"=>598,
    "user_id"=>27461,
    "ago"=>"5m",
    "post"=>
     {"id"=>1915,
      "title"=>"Polarised full-range moderator: Small Plastic Gloves",
      "excerpt"=>"Triple-buffered holistic pricing structure",
      "group"=>nil,
      "event"=>{"id"=>4286, "name"=>"Awesome Cotton Table 318"}}}]}
```

This requests provides a <strong>HTML 200</strong> on success.