<!-- --- title: GET /groups -->

Returns a list of all groups that are visible to the active user. Secret groups that the user is not a member of will not be returned. 

=
#### Authentication

The user needs to be logged in and have valid credentials to use this route.

=
#### Parameters

none; default only

=
####JSON request example:
```json
http://stage-api-access.evant.com/groups
```

=
####JSON response example:

```json
{"groups"=>
  [{"id"=>1,
    "name"=>"Open Group 1",
    "description"=>"Open group 1",
    "owner_user_id"=>2,
    "member_count"=>5,
    "group_member_id"=>nil,
    "group_request_id"=>nil,
    "group_request_is_approved"=>nil,
    "group_invite_id"=>nil,
    "create_post"=>false,
    "leave_group"=>true,
    "hide_app_sponsors"=>false,
    "group_type"=>
     {"id"=>1,
      "name"=>"Factory:Open",
      "description"=>"Open",
      "is_group_visible"=>true,
      "is_memberlist_visible"=>true,
      "is_content_visible"=>true,
      "is_approval_required"=>false},
    "owner"=>
     {"id"=>2,
      "first_name"=>"Group",
      "last_name"=>"Owner",
      "title"=>"Group Owner",
      "organization_name"=>"Carroll, Nicolas and Daniel",
      "photo"=>
       "https://assets.evanta.com/shared/resources/Users/large/anonymous2.jpg",
      "user_role_id"=>1,
      "user_connections_blocked"=>false,
      "user_profile"=>true,
      "event_council_member"=>false,
      "connection_status"=>nil},
    "group_sponsors"=>[],
    "group_members"=>
     [{"id"=>1,
       "group_id"=>1,
       "user"=>
        {"id"=>11,
         "first_name"=>"AAA",
         "last_name"=>"AAA",
         "title"=>
          "Legacy Communications Associate of Clothing, Shoes & Jewelery",
         "organization_name"=>"Ebert LLC",
         "photo"=>
          "https://assets.evanta.com/shared/resources/Users/large/anonymous2.jpg",
         "user_role_id"=>1,
         "user_connections_blocked"=>false,
         "user_profile"=>true,
         "event_council_member"=>false,
         "connection_status"=>
          {"id"=>1, "is_approved"=>true, "is_approver"=>false}}},
      {"id"=>2,
       "group_id"=>1,
       "user"=>
        {"id"=>12,
         "first_name"=>"BBB",
         "last_name"=>"AAA",
         "title"=>"Senior Program Executive of Automotive & Industrial",
         "organization_name"=>"Wilderman-Ziemann",
         "photo"=>
          "https://assets.evanta.com/shared/resources/Users/large/anonymous2.jpg",
         "user_role_id"=>1,
         "user_connections_blocked"=>false,
         "user_profile"=>true,
         "event_council_member"=>false,
         "connection_status"=>
          {"id"=>2, "is_approved"=>false, "is_approver"=>false}}},
      {"id"=>3,
       "group_id"=>1,
       "user"=>
        {"id"=>13,
         "first_name"=>"CCC",
         "last_name"=>"CCC",
         "title"=>
          "National Implementation Facilitator of Electronics & Computers",
         "organization_name"=>"Hettinger, Sipes and Stamm",
         "photo"=>
          "https://assets.evanta.com/shared/resources/Users/large/anonymous2.jpg",
         "user_role_id"=>1,
         "user_connections_blocked"=>false,
         "user_profile"=>true,
         "event_council_member"=>false,
         "connection_status"=>
          {"id"=>3, "is_approved"=>true, "is_approver"=>false}}},
      {"id"=>4,
       "group_id"=>1,
       "user"=>
        {"id"=>14,
         "first_name"=>"DDD",
         "last_name"=>"DDD",
         "title"=>"Direct Communications Associate of Sports & Outdoors",
         "organization_name"=>"Cummerata Inc",
         "photo"=>
          "https://assets.evanta.com/shared/resources/Users/large/anonymous2.jpg",
         "user_role_id"=>1,
         "user_connections_blocked"=>false,
         "user_profile"=>true,
         "event_council_member"=>false,
         "connection_status"=>nil}},
      {"id"=>5,
       "group_id"=>1,
       "user"=>
        {"id"=>15,
         "first_name"=>"EEE",
         "last_name"=>"EEE",
         "title"=>
          "Customer Communications Representative of Movies, Music & Games",
         "organization_name"=>"McCullough Group",
         "photo"=>
          "https://assets.evanta.com/shared/resources/Users/large/anonymous2.jpg",
         "user_role_id"=>1,
         "user_connections_blocked"=>false,
         "user_profile"=>true,
         "event_council_member"=>false,
         "connection_status"=>nil}}],
    "group_invites"=>[],
    "group_requests"=>[]},
   {"id"=>2,
    "name"=>"Private Group 1",
    "description"=>"Private group 1",
    "owner_user_id"=>5,
    "member_count"=>0,
    "group_member_id"=>nil,
    "group_request_id"=>nil,
    "group_request_is_approved"=>nil,
    "group_invite_id"=>nil,
    "create_post"=>false,
    "leave_group"=>true,
    "hide_app_sponsors"=>false,
    "group_type"=>
     {"id"=>2,
      "name"=>"Factory:Private",
      "description"=>"Private",
      "is_group_visible"=>true,
      "is_memberlist_visible"=>false,
      "is_content_visible"=>false,
      "is_approval_required"=>true},
    "owner"=>
     {"id"=>5,
      "first_name"=>"Group",
      "last_name"=>"Owner",
      "title"=>"Group Owner",
      "organization_name"=>"Cruickshank, Mitchell and Kohler",
      "photo"=>
       "https://assets.evanta.com/shared/resources/Users/large/anonymous2.jpg",
      "user_role_id"=>1,
      "user_connections_blocked"=>false,
      "user_profile"=>true,
      "event_council_member"=>false,
      "connection_status"=>nil},
    "group_sponsors"=>[],
    "group_members"=>[],
    "group_invites"=>[],
    "group_requests"=>[]}]}
```

This requests provides a <strong>HTML 200</strong> on success.