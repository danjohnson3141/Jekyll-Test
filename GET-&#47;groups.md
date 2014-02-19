Returns a list of all groups.

=
#### Authentication

The user needs to be logged in and have valid credentials to use this route.

=
#### Parameters

none; default only

=
####JSON request example:
```
http://0.0.0.0:3000/groups
```

=
####JSON response example:

```
{"groups"=>
  [{"id"=>3173,
    "name"=>"Incredible Granite Table",
    "description"=>
     "Blanditiis dolor labore nemo necessitatibus libero eveniet culpa impedit debitis.",
    "owner_user_id"=>25427,
    "app_sponsor_id"=>1533,
    "member_count"=>0,
    "group_member_id"=>nil,
    "group_request_id"=>nil,
    "group_request_is_approved"=>nil,
    "group_invite_id"=>nil,
    "create_groups"=>nil,
    "leave_group"=>nil,
    "banner_ads"=>[],
    "group_type"=>
     {"id"=>5751,
      "name"=>"Factory:Open",
      "description"=>"Open",
      "is_group_visible"=>true,
      "is_memberlist_visible"=>true,
      "is_content_visible"=>true,
      "is_approval_required"=>false},
    "app_sponsor"=>
     {"id"=>1533,
      "name"=>"Roob-Bernier",
      "description"=>
       "Aut sed ea sit necessitatibus iure velit aut voluptatibus est non.",
      "logo"=>"www.example.com/app_sponsor_logo.jpg",
      "url"=>"trompkuhic.org",
      "primary_app_sponsor"=>false,
      "sponsor_type"=>
       {"id"=>1895,
        "name"=>"cyan",
        "description"=>"Pre-emptive zero tolerance analyzer"},
      "users"=>[]},
    "owner"=>
     {"id"=>25427,
      "first_name"=>"Einar",
      "last_name"=>"Welch",
      "title"=>"Creator Of All 1",
      "organization_name"=>"Aufderhar, Paucek and Pfannerstill",
      "photo"=>
       "https://assets.evanta.com/shared/resources/Users/large/anonymous2.jpg",
      "user_role_id"=>25431,
      "user_connection_id"=>nil}},
   {"id"=>3172,
    "name"=>"Practical Granite Pants",
    "description"=>"Maiores sed cupiditate rerum in dolore eaque.",
    "owner_user_id"=>25424,
    "app_sponsor_id"=>1532,
    "member_count"=>0,
    "group_member_id"=>nil,
    "group_request_id"=>nil,
    "group_request_is_approved"=>nil,
    "group_invite_id"=>nil,
    "create_groups"=>nil,
    "leave_group"=>nil,
    "banner_ads"=>[],
    "group_type"=>
     {"id"=>5750,
      "name"=>"Factory:Open",
      "description"=>"Open",
      "is_group_visible"=>true,
      "is_memberlist_visible"=>true,
      "is_content_visible"=>true,
      "is_approval_required"=>false},
    "app_sponsor"=>
     {"id"=>1532,
      "name"=>"Hoeger, Cummerata and Rosenbaum",
      "description"=>
       "Totam pariatur voluptates suscipit eaque distinctio blanditiis quia ut dicta vero aperiam vitae.",
      "logo"=>"www.example.com/app_sponsor_logo.jpg",
      "url"=>"pfefferstanton.com",
      "primary_app_sponsor"=>false,
      "sponsor_type"=>
       {"id"=>1894,
        "name"=>"yellow",
        "description"=>"Balanced demand-driven local area network"},
      "users"=>[]},
    "owner"=>
     {"id"=>25424,
      "first_name"=>"Hanna",
      "last_name"=>"Weimann",
      "title"=>"Creator Of All 1",
      "organization_name"=>"Boyle Group",
      "photo"=>
       "https://assets.evanta.com/shared/resources/Users/large/anonymous2.jpg",
      "user_role_id"=>25428,
      "user_connection_id"=>nil}}]}
```

This requests provides a <strong>HTML RESPONSE NUMBER</strong> on success.