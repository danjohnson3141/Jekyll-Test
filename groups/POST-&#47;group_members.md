<!-- --- title: POST /group_members -->

This creates a new group membership record. The user associated with this record will always be the active user.

=
####Authentication

The user needs to be logged in and have valid credentials to use this route. This is the group that the active user will now be a member of.

=
####Parameters

:group_id - Integer, passed in through the post data. Is derived from the 'id' field on the 'groups' table.

=
####Post Data
```
{ group_member: 
  { group_id: 296 } 
```

=
####JSON request example:
```
http://0.0.0.0:3000/group_members
```

=
####JSON response example:

```
{"group_member"=>
  {"id"=>42,
   "created_by"=>nil,
   "updated_by"=>nil,
   "user"=>
    {"id"=>2154,
     "email"=>"generic_user@evanta.com",
     "alt_email"=>nil,
     "first_name"=>"Generic",
     "last_name"=>"User",
     "title"=>"CEO of QA",
     "organization_name"=>"Evanta",
     "bio"=>nil,
     "photo"=>
      "https://assets.evanta.com/shared/resources/Users/large/anonymous2.jpg",
     "user_role_id"=>2158,
     "user_connection_id"=>nil},
   "group"=>
    {"id"=>296,
     "name"=>"TestGroup",
     "description"=>"For Testing",
     "owner_user_id"=>nil,
     "app_sponsor_id"=>nil,
     "member_count"=>1,
     "group_member_id"=>42,
     "group_request_id"=>nil,
     "group_request_is_approved"=>nil,
     "group_invite_id"=>nil,
     "create_groups"=>nil,
     "leave_group"=>nil,
     "banner_ads"=>[],
     "group_type"=>
      {"id"=>499,
       "name"=>"Factory:Open",
       "description"=>"Open",
       "is_group_visible"=>true,
       "is_memberlist_visible"=>true,
       "is_content_visible"=>true,
       "is_approval_required"=>false},
     "app_sponsor"=>nil,
     "owner"=>nil}}}
```

This requests provides a <strong>HTML 201</strong> on success.