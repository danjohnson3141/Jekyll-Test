<!-- --- title: GET /group_members/groups/:user_id -->

This returns a list of all the groups that a user is a member of. 

=
####Authentication:

The user needs to be logged in and have valid credentials to use this route.

=
####Parameters:

:user_id - Integer, passed in through the URL. Is derived from the 'id' field on the 'users' table.

=
####Response:

This requests provides a <strong>HTML 200</strong> on success.

=
####API request example:
```json
http://stage-api-access.evant.com/group_members/groups/13175
```

=
####JSON response example:

```json
{"group_members"=>
  [{"id"=>277,
    "user_id"=>13175,
    "group"=>
     {"id"=>1619,
      "name"=>"Incredible Rubber Table",
      "description"=>"Magni tempore aliquam velit voluptas et.",
      "owner_user_id"=>13178,
      "app_sponsor_id"=>782,
      "member_count"=>1,
      "group_member_id"=>nil,
      "group_request_id"=>nil,
      "group_request_is_approved"=>nil,
      "group_invite_id"=>nil,
      "create_groups"=>nil,
      "leave_group"=>nil,
      "banner_ads"=>[],
      "group_type"=>
       {"id"=>2986,
        "name"=>"Factory:Open",
        "description"=>"Open",
        "is_group_visible"=>true,
        "is_memberlist_visible"=>true,
        "is_content_visible"=>true,
        "is_approval_required"=>false},
      "app_sponsor"=>
       {"id"=>782,
        "name"=>"Buckridge-Labadie",
        "description"=>
         "Reiciendis ut quae et similique commodi nisi repudiandae delectus aspernatur provident est.",
        "logo"=>"www.example.com/app_sponsor_logo.jpg",
        "url"=>"beerhaley.name",
        "primary_app_sponsor"=>false,
        "sponsor_type"=>
         {"id"=>942,
          "name"=>"red",
          "description"=>"Operative bi-directional methodology"},
        "users"=>[]},
      "owner"=>
       {"id"=>13178,
        "first_name"=>"Delphia",
        "last_name"=>"Schmitt",
        "title"=>"Creator Of All 1",
        "organization_name"=>"Altenwerth-Jakubowski",
        "photo"=>
         "https://assets.evanta.com/shared/resources/Users/large/anonymous.jpg",
        "user_role_id"=>13182,
        "user_connection_id"=>nil}}},
   {"id"=>278,
    "user_id"=>13175,
    "group"=>
     {"id"=>1620,
      "name"=>"Ergonomic Plastic Chair",
      "description"=>"Facilis quis suscipit magnam ut.",
      "owner_user_id"=>13181,
      "app_sponsor_id"=>783,
      "member_count"=>1,
      "group_member_id"=>nil,
      "group_request_id"=>nil,
      "group_request_is_approved"=>nil,
      "group_invite_id"=>nil,
      "create_groups"=>nil,
      "leave_group"=>nil,
      "banner_ads"=>[],
      "group_type"=>
       {"id"=>2987,
        "name"=>"Factory:Open",
        "description"=>"Open",
        "is_group_visible"=>true,
        "is_memberlist_visible"=>true,
        "is_content_visible"=>true,
        "is_approval_required"=>false},
      "app_sponsor"=>
       {"id"=>783,
        "name"=>"Boyle, Ritchie and Waters",
        "description"=>
         "Ea quo et dicta et quaerat nulla et expedita aut sunt quisquam quis sint voluptas.",
        "logo"=>"www.example.com/app_sponsor_logo.jpg",
        "url"=>"hermanfahey.com",
        "primary_app_sponsor"=>false,
        "sponsor_type"=>
         {"id"=>943,
          "name"=>"green",
          "description"=>"Synchronised full-range system engine"},
        "users"=>[]},
      "owner"=>
       {"id"=>13181,
        "first_name"=>"Alfonzo",
        "last_name"=>"Wiegand",
        "title"=>"Creator Of All 1",
        "organization_name"=>"Weimann LLC",
        "photo"=>
         "https://assets.evanta.com/shared/resources/Users/large/anonymous.jpg",
        "user_role_id"=>13185,
        "user_connection_id"=>nil}}}]}
```