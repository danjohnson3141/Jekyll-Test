<!-- --- title: GET /group_invites/groups -->

This route returns all of the pending invites for the active user. Should not return invites for groups that the user is already a member of.

=
####Authentication:

The user needs to be logged in and have valid credentials to use this route.

=
####Parameters:

None; default only.

=
####Response:

This requests provides a <strong>HTML 200</strong> on success.

=
####API request example:
```json
http://stage-api-access.evant.com/group_invites/groups
```

=
####JSON response example:

[[include:/json/JSON_GET_groups_id]]

=
####Response Data Detail:

[[include:/serializers/group_invite_group]]