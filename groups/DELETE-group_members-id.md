<!-- --- title: DELETE /group_members/:id -->

Allows the user to delete their group membership. Only the user is able to delete group memberships and only for the their own memberships. 

=
####Authentication:

The user needs to be logged in and have valid credentials to use this route.

=
####Parameters:

:id - Integer, passed in through the URL. Is derived from the 'id' field on the 'group_members' table.

=
####Response:

This requests provides a <strong>HTML 204</strong> on success.

=
####API request example:
```
http://stage-api-access.evant.com/group_members/234
```

=
####JSON response example:

[[include:/json/JSON_NO_RESPONSE]]