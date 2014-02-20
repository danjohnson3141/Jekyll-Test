Creates an invitation for another user to join a group. Only the owner of a group is allowed to create invitations.

=
#### Authentication

The user needs to be logged in and have valid credentials to use this route.

=
#### Parameters

:group_id - Integer, passed in through the post data. Is derived from the 'id' field on the 'groups' table. This is the ID of the group that the invite will be associated with.

:user_id - Integer, passed in through the post data. Derived from the 'id' field of the 'users' table. This is who the invitation will be sent to.

=
####JSON request example:
```
http://0.0.0.0:3000/group_invites
```

=
####Post Data
```
{ group_invite: 
  { user_id: @user.id, 
    group_id: group.id } 
 }
```

=
####JSON response example:

```
{"group_invite"=>
  {"id"=>486,
   "user"=>
    {"id"=>28187,
     "email"=>"generic_user@evanta.com",
     "alt_email"=>nil,
     "first_name"=>"Generic",
     "last_name"=>"User",
     "title"=>"CEO of QA",
     "organization_name"=>"Evanta",
     "bio"=>nil,
     "photo"=>
      "https://assets.evanta.com/shared/resources/Users/large/anonymous2.jpg",
     "user_role_id"=>28191,
     "user_connection_id"=>nil},
   "group"=>
    {"id"=>3563,
     "name"=>"Private Group",
     "description"=>"Private group",
     "owner_user_id"=>28187,
     "app_sponsor_id"=>nil,
     "member_count"=>0,
     "group_member_id"=>nil,
     "group_request_id"=>nil,
     "group_request_is_approved"=>nil,
     "group_invite_id"=>486,
     "create_groups"=>nil,
     "leave_group"=>nil,
     "banner_ads"=>[],
     "group_type"=>
      {"id"=>6407,
       "name"=>"Factory:Private",
       "description"=>"Private",
       "is_group_visible"=>true,
       "is_memberlist_visible"=>false,
       "is_content_visible"=>false,
       "is_approval_required"=>true},
     "app_sponsor"=>nil,
     "owner"=>
      {"id"=>28187,
       "first_name"=>"Generic",
       "last_name"=>"User",
       "title"=>"CEO of QA",
       "organization_name"=>"Evanta",
       "photo"=>
        "https://assets.evanta.com/shared/resources/Users/large/anonymous2.jpg",
       "user_role_id"=>28191,
       "user_connection_id"=>nil}}}}
```

This requests provides a <strong>HTML RESPONSE NUMBER</strong> on success.