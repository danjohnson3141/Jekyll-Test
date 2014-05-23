<!-- --- title: GET /group_requests/users/:group_id -->

Returns a list of all the group requests for **one** group. Should not return any users who are members of the group. The active user needs to be the group owner for this route to work.

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
http://stage-api-access.evant.com/group_requests/users/1917
```

=
####JSON response example:

Returns an array of user objects

[[include:/json/JSON_GET_group_requests_users_group_id]]

=
####Response Data Detail:

[[include:/serializers/group_request_user]]