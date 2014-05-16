<!-- --- title: POST /group_invites -->

Creates an invitation for another user to join a group. Only the owner of a group is allowed to create invitations for that group

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
####Post data example:
```
{ group_invite: 
  { user_id: 29845, 
    group_id: 3773 } 
 }
```

=
###Post data detail:

[[include:/post_data/post_group_invites]]

=
####JSON response example:

[[include:/json/JSON_POST_group_invites]]

=
####Response Data Detail:

[[include:/serializers/group_invite]]