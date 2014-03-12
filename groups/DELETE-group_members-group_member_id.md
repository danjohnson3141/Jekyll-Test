<!-- --- title: DELETE /group_members/:group_member_id -->

Allows the user to delete their group membership. Only the user is able to delete group memberships and only for the their own memberships. 

=
#### Authentication

The user needs to be logged in and have valid credentials to use this route.

=
#### Parameters

:group_members_id - Integer, passed in through the URL. Is derived from the 'id' field on the 'group_members' table.

=
####JSON request example:

```
http://0.0.0.0:3000/group_members/234
```

=
####JSON response example:

```json
NO JSON RESPONSE
```

This requests provides a <strong>HTML 204</strong> on success.