Returns details on **one** group.

=
#### Authentication

The user needs to be logged in and have valid credentials to use this route.

=
#### Parameters

:group_id - Integer, passed in through the URL. Is derived from the 'id' field on the 'groups' table.

=
####JSON request example:
```
http://0.0.0.0:3000/ROUTE_NAME
```

=
####JSON response example:

```
{"group"=>
  {"id"=>2315,
   "name"=>"Rustic Cotton Hat",
   "description"=>
    "Facilis voluptates qui enim sapiente aut nemo occaecati iste.",
   "owner_user_id"=>18757,
   "app_sponsor_id"=>1112,
   "member_count"=>0,
   "group_member_id"=>nil,
   "group_request_id"=>nil,
   "group_request_is_approved"=>nil,
   "group_invite_id"=>nil,
   "create_groups"=>nil,
   "leave_group"=>nil,
   "banner_ads"=>[],
   "group_type"=>
    {"id"=>4289,
     "name"=>"Factory:Open",
     "description"=>"Open",
     "is_group_visible"=>true,
     "is_memberlist_visible"=>true,
     "is_content_visible"=>true,
     "is_approval_required"=>false},
   "app_sponsor"=>
    {"id"=>1112,
     "name"=>"Gerhold-Lakin",
     "description"=>
      "Sed eos voluptatibus at voluptatum totam ut aspernatur dolores amet pariatur quisquam aut dolore.",
     "logo"=>"www.example.com/app_sponsor_logo.jpg",
     "url"=>"reichelfahey.org",
     "primary_app_sponsor"=>false,
     "sponsor_type"=>
      {"id"=>1345,
       "name"=>"azure",
       "description"=>"Grass-roots intermediate emulation"},
     "users"=>[]},
   "owner"=>
    {"id"=>18757,
     "first_name"=>"Travis",
     "last_name"=>"Witting",
     "title"=>"Creator Of All 1",
     "organization_name"=>"Ferry LLC",
     "photo"=>
      "https://assets.evanta.com/shared/resources/Users/large/anonymous.jpg",
     "user_role_id"=>18761,
     "user_connection_id"=>nil}}}
```

This requests provides a <strong>HTML 200</strong> on success.