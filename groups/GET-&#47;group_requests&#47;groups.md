<!-- --- title: GET /group_requests/groups -->

Returns all of the outstanding requests for the logged in user. Should not return any groups that the user is already a member of.

=
#### Authentication

The user needs to be logged in and have valid credentials to use this route.

=
#### Parameters

none; default only

=
####JSON request example:
```
http://0.0.0.0:3000/group_requests/groups
```

=
####JSON response example:

```json
{"group_members"=>
  [{"id"=>298,
    "user_id"=>14164,
    "group"=>
     {"id"=>1745,
      "name"=>"Ergonomic Plastic Computer",
      "description"=>
       "Dolor reprehenderit quis enim consequuntur quae praesentium.",
      "owner_user_id"=>14167,
      "app_sponsor_id"=>840,
      "member_count"=>1,
      "group_member_id"=>nil,
      "group_request_id"=>nil,
      "group_request_is_approved"=>nil,
      "group_invite_id"=>nil,
      "create_groups"=>nil,
      "leave_group"=>nil,
      "banner_ads"=>[],
      "group_type"=>
       {"id"=>3203,
        "name"=>"Factory:Open",
        "description"=>"Open",
        "is_group_visible"=>true,
        "is_memberlist_visible"=>true,
        "is_content_visible"=>true,
        "is_approval_required"=>false},
      "app_sponsor"=>
       {"id"=>840,
        "name"=>"Connelly, Rau and O'Connell",
        "description"=>
         "Ut doloribus asperiores fuga dolor inventore ipsa enim voluptas voluptatem iure quidem eligendi.",
        "logo"=>"www.example.com/app_sponsor_logo.jpg",
        "url"=>"bradtke.org",
        "primary_app_sponsor"=>false,
        "sponsor_type"=>
         {"id"=>1014,
          "name"=>"gold",
          "description"=>"Horizontal bi-directional Graphical User Interface"},
        "users"=>[]},
      "owner"=>
       {"id"=>14167,
        "first_name"=>"Enrique",
        "last_name"=>"Hackett",
        "title"=>"Creator Of All 1",
        "organization_name"=>"Leffler, Kshlerin and Rowe",
        "photo"=>
         "https://assets.evanta.com/shared/resources/Users/large/anonymous.jpg",
        "user_role_id"=>14171,
        "user_connection_id"=>nil}}},
   {"id"=>299,
    "user_id"=>14164,
    "group"=>
     {"id"=>1746,
      "name"=>"Rustic Rubber Gloves",
      "description"=>"Nam cupiditate deserunt dolorem at occaecati amet.",
      "owner_user_id"=>14170,
      "app_sponsor_id"=>841,
      "member_count"=>1,
      "group_member_id"=>nil,
      "group_request_id"=>nil,
      "group_request_is_approved"=>nil,
      "group_invite_id"=>nil,
      "create_groups"=>nil,
      "leave_group"=>nil,
      "banner_ads"=>[],
      "group_type"=>
       {"id"=>3204,
        "name"=>"Factory:Open",
        "description"=>"Open",
        "is_group_visible"=>true,
        "is_memberlist_visible"=>true,
        "is_content_visible"=>true,
        "is_approval_required"=>false},
      "app_sponsor"=>
       {"id"=>841,
        "name"=>"Senger Group",
        "description"=>
         "Laborum ut consequatur id accusantium iusto culpa dolorum aut vitae.",
        "logo"=>"www.example.com/app_sponsor_logo.jpg",
        "url"=>"quigleyreichel.net",
        "primary_app_sponsor"=>false,
        "sponsor_type"=>
         {"id"=>1015,
          "name"=>"plum",
          "description"=>"Exclusive transitional orchestration"},
        "users"=>[]},
      "owner"=>
       {"id"=>14170,
        "first_name"=>"Jayden",
        "last_name"=>"Mohr",
        "title"=>"Creator Of All 1",
        "organization_name"=>"Kutch, Fay and Block",
        "photo"=>
         "https://assets.evanta.com/shared/resources/Users/large/anonymous.jpg",
        "user_role_id"=>14174,
        "user_connection_id"=>nil}}}]}
```

This requests provides a <strong>HTML 200</strong> on success.