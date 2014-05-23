<!-- --- title: GET /group_invites/users/:group_id -->

Returns all of the pending user invites for a group. Should not return any invites for users who members of the group. Should only return any values if the user is the owner of the group.

=
####Authentication:

The user needs to be logged in and have valid credentials to use this route.

=
####Parameters:

:group_id - Integer, passed in through the URL. Is derived from the 'id' field on the 'groups' table.

=
####Response:

This requests provides a <strong>HTML 200</strong> on success.

=
####API request example:
```html
http://stage-api-access.evant.com/group_invites/users/1158
```

=
####JSON response example:

[[include:/json/JSON_GET_group_invites_users_group_id]]

=
####Response Data Detail:

[[include:/serializers/group_invite_user]]