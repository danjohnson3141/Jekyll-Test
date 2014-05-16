<!-- --- title: GET /group_members/groups/:user_id -->

This returns a list of all the groups that a user is a member of. 

=
####Authentication:

The user needs to be logged in and have valid credentials to use this route.

=
####Parameters:

:user_id - Integer, passed in through the URL. Is derived from the 'id' field on the 'users' table.

=
####Response:

This requests provides a <strong>HTML 200</strong> on success.

=
####API request example:
```json
http://stage-api-access.evant.com/group_members/groups/13175
```

=
####JSON response example:

[[include:/json/JSON_GET_group_members_groups_user_user_id]]

=
####Response Data Detail:

[[include:/serializers/group_members_group]]