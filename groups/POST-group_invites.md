<!-- --- title: POST /group_invites -->

Creates an invitation for another user to join a group. Only the owner of a group is allowed to create invitations.

=
####Authentication:

The user needs to be logged in and have valid credentials to use this route.

=
####Parameters:

:group_id - Integer, passed in through the post data. Is derived from the 'id' field on the 'groups' table. This is the ID of the group that the invite will be associated with.

:user_id - Integer, passed in through the post data. Derived from the 'id' field of the 'users' table. This is who the invitation will be sent to.

=
####Response:

This requests provides a <strong>HTML 201</strong> on success.

=
####API request example:
```json
http://stage-api-access.evant.com/group_invites
```

=
####Post Data:
```
{ group_invite: 
  { user_id: 29845, 
    group_id: 3773 } 
 }
```

=
####JSON response example:

```json
{"group_invite"=>
  {"id"=>506,
   "user"=>
    {"id"=>29845,
     "email"=>"juliet@towne.com",
     "alt_email"=>"davonte_gleichner@hotmail.com",
     "first_name"=>"Sonny",
     "last_name"=>"Tromp",
     "title"=>"Random User",
     "organization_name"=>"Bailey Inc",
     "bio"=>"Et qui aut veritatis quo omnis et voluptas quia ipsa nulla.",
     "photo"=>
      "https://assets.evanta.com/shared/resources/Users/large/anonymous2.jpg",
     "user_role_id"=>29847,
     "user_connection_id"=>nil},
   "group"=>
    {"id"=>3773,
     "name"=>"Private Group",
     "description"=>"Private group",
     "owner_user_id"=>29842,
     "app_sponsor_id"=>nil,
     "member_count"=>0,
     "group_member_id"=>nil,
     "group_request_id"=>nil,
     "group_request_is_approved"=>nil,
     "group_invite_id"=>nil,
     "create_groups"=>nil,
     "leave_group"=>nil,
     "banner_ads"=>[],
     "group_type"=>
      {"id"=>6772,
       "name"=>"Factory:Private",
       "description"=>"Private",
       "is_group_visible"=>true,
       "is_memberlist_visible"=>false,
       "is_content_visible"=>false,
       "is_approval_required"=>true},
     "app_sponsor"=>nil,
     "owner"=>
      {"id"=>29842,
       "first_name"=>"Generic",
       "last_name"=>"User",
       "title"=>"CEO of QA",
       "organization_name"=>"Evanta",
       "photo"=>
        "https://assets.evanta.com/shared/resources/Users/large/anonymous2.jpg",
       "user_role_id"=>29846,
       "user_connection_id"=>nil}}}}
```