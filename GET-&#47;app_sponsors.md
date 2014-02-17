This returns a list of **ALL** sponsors.

=
#### Authentication
The user needs to be logged in and have valid credentials to use this route.

=
#### Parameters

LIST OF ALL PARAMETERS AND WHAT THEY ARE

=
####JSON request example:

```
http://0.0.0.0:3000/app_sponsors
```

=
####JSON response example:

```
{"app_sponsors"=>
  [{"id"=>27,
    "name"=>"Pfeffer-Rogahn",
    "description"=>
     "Sapiente cupiditate dolores voluptatem ut animi aut iure sint qui quasi voluptatem occaecati consequatur ut.",
    "logo"=>"www.example.com/app_sponsor_logo.jpg",
    "url"=>"moore.biz",
    "primary_app_sponsor"=>false,
    "sponsor_type"=>
     {"id"=>65,
      "name"=>"cyan",
      "description"=>"User-friendly asynchronous local area network"},
    "users"=>
     [{"id"=>2338,
       "first_name"=>"Earnestine",
       "last_name"=>"Romaguera",
       "title"=>"Random User",
       "organization_name"=>"Littel-Leffler",
       "photo"=>"www.example.com/user_photo.jpg",
       "user_role_id"=>2342,
       "user_connection_id"=>66}]},
   {"id"=>28,
    "name"=>"Hansen-Pouros",
    "description"=>
     "Ut earum tenetur provident mollitia facere ut perspiciatis consequatur qui minima laboriosam assumenda incidunt omnis.",
    "logo"=>"www.example.com/app_sponsor_logo.jpg",
    "url"=>"moorehammes.info",
    "primary_app_sponsor"=>false,
    "sponsor_type"=>
     {"id"=>66,
      "name"=>"ivory",
      "description"=>"Progressive 4th generation analyzer"},
    "users"=>
     [{"id"=>2339,
       "first_name"=>"Damion",
       "last_name"=>"Harvey",
       "title"=>"Random User",
       "organization_name"=>"Predovic, Leffler and Bogan",
       "photo"=>"www.example.com/user_photo.jpg",
       "user_role_id"=>2343,
       "user_connection_id"=>67}]}]}
```

This requests provides a <strong>HTML RESPONSE NUMBER</strong> on success.