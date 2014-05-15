<!-- --- title: POST /group_requests -->

This creates a new record for the user trying to join a group that requires approval to join.

=
####Authentication:

The user needs to be logged in and have valid credentials to use this route.

=
####Parameters:

:group_id - Integer, passed in through the post data. Is derived from the 'id' field on the 'groups' table. This is the group that the user is requesting to join.

:user_id - Integer, passed in through the post data. Derived from the 'id' field of the 'users' table.

=
####Response:

This requests provides a <strong>HTML 201</strong> on success.

=
####API request example:
```json
http://stage-api-access.evant.com/group_requests
```

=
####Post Data:
```
{ group_request: 
  { user_id: 5317, 
    group_id: 706 } 
 }
```

=
####JSON response example:

```json
{"group_request"=>
  {"id"=>89,
   "user"=>
    {"id"=>5317,
     "email"=>"generic_user@evanta.com",
     "alt_email"=>nil,
     "first_name"=>"Generic",
     "last_name"=>"User",
     "title"=>"CEO of QA",
     "organization_name"=>"Evanta",
     "bio"=>"This is the biography of the default Generic User",
     "photo"=>
      "https://assets.evanta.com/shared/resources/Users/large/anonymous2.jpg",
     "user_role_id"=>5321,
     "user_connection_id"=>nil},
   "group"=>
    {"id"=>706,
     "name"=>"TestGroup",
     "description"=>"For Testing",
     "owner_user_id"=>nil,
     "member_count"=>0,
     "group_member_id"=>nil,
     "group_request_id"=>89,
     "group_request_is_approved"=>false,
     "group_invite_id"=>nil,
     "create_post"=>false,
     "create_groups"=>nil,
     "leave_group"=>nil,
     "group_type"=>
      {"id"=>1181,
       "name"=>"Factory:Open",
       "description"=>"Open",
       "is_group_visible"=>true,
       "is_memberlist_visible"=>true,
       "is_content_visible"=>true,
       "is_approval_required"=>false},
     "owner"=>nil,
     "banner_ads"=>[],
     "group_sponsor"=>nil,
     "group_members"=>[]}}}
```