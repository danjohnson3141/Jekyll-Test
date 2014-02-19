This route returns all of the pending invites for the logged in user. Should not return invites for groups that the user is already a member of.

=
#### Authentication

The user needs to be logged in and have valid credentials to use this route.

=
#### Parameters

none; default only

=
####JSON request example:
```
http://0.0.0.0:3000/ROUTE_NAME
```

=
####JSON response example:

```
{"group_invites"=>
  [{"id"=>122,
    "user_id"=>7021,
    "group"=>
     {"id"=>837,
      "name"=>"Practical Concrete Computer",
      "description"=>
       "Aut consequatur aut repudiandae aut quasi tempore dolore.",
      "owner_user_id"=>7027,
      "app_sponsor_id"=>401,
      "member_count"=>0,
      "group_member_id"=>nil,
      "group_request_id"=>nil,
      "group_request_is_approved"=>nil,
      "group_invite_id"=>122,
      "create_groups"=>nil,
      "leave_group"=>nil,
      "banner_ads"=>[],
      "group_type"=>
       {"id"=>1593,
        "name"=>"Factory:Open",
        "description"=>"Open",
        "is_group_visible"=>true,
        "is_memberlist_visible"=>true,
        "is_content_visible"=>true,
        "is_approval_required"=>false},
      "app_sponsor"=>
       {"id"=>401,
        "name"=>"Kshlerin-Fritsch",
        "description"=>
         "Excepturi repellendus quia quos aperiam dicta iste quaerat doloremque voluptas magnam praesentium ea.",
        "logo"=>"www.example.com/app_sponsor_logo.jpg",
        "url"=>"kub.biz",
        "primary_app_sponsor"=>false,
        "sponsor_type"=>
         {"id"=>477,
          "name"=>"pink",
          "description"=>"Integrated maximized emulation"},
        "users"=>[]},
      "owner"=>
       {"id"=>7027,
        "first_name"=>"Kendall",
        "last_name"=>"Kunze",
        "title"=>"Creator Of All 1",
        "organization_name"=>"Schulist-Rodriguez",
        "photo"=>
         "https://assets.evanta.com/shared/resources/Users/large/anonymous.jpg",
        "user_role_id"=>7031,
        "user_connection_id"=>nil}}},
   {"id"=>121,
    "user_id"=>7021,
    "group"=>
     {"id"=>836,
      "name"=>"Rustic Granite Pants",
      "description"=>"Ad fugit rem sit aut enim voluptate qui.",
      "owner_user_id"=>7024,
      "app_sponsor_id"=>400,
      "member_count"=>0,
      "group_member_id"=>nil,
      "group_request_id"=>nil,
      "group_request_is_approved"=>nil,
      "group_invite_id"=>121,
      "create_groups"=>nil,
      "leave_group"=>nil,
      "banner_ads"=>[],
      "group_type"=>
       {"id"=>1592,
        "name"=>"Factory:Open",
        "description"=>"Open",
        "is_group_visible"=>true,
        "is_memberlist_visible"=>true,
        "is_content_visible"=>true,
        "is_approval_required"=>false},
      "app_sponsor"=>
       {"id"=>400,
        "name"=>"Fay, Klein and O'Conner",
        "description"=>
         "Consectetur quibusdam sit quod quo dolor omnis est nulla et est laudantium a odit.",
        "logo"=>"www.example.com/app_sponsor_logo.jpg",
        "url"=>"greendare.net",
        "primary_app_sponsor"=>false,
        "sponsor_type"=>
         {"id"=>476,
          "name"=>"black",
          "description"=>"Cloned holistic functionalities"},
        "users"=>[]},
      "owner"=>
       {"id"=>7024,
        "first_name"=>"Ramiro",
        "last_name"=>"Hane",
        "title"=>"Creator Of All 1",
        "organization_name"=>"Jenkins and Sons",
        "photo"=>
         "https://assets.evanta.com/shared/resources/Users/large/anonymous.jpg",
        "user_role_id"=>7028,
        "user_connection_id"=>nil}}}]}
```

This requests provides a <strong>HTML RESPONSE NUMBER</strong> on success.