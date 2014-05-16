<!-- --- title: GET /group_members/users/:group_id -->

Returns a list of all of the members of a group.

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
```json
http://stage-api-access.evant.com/group_members/users/1671
```

=
####JSON response example:

Returns an array of user objects

[[include:/json/JSON_GET_group_members_users_group_id]]

=
####Response Data Detail:

[[include:/serializers/group_members_user]]