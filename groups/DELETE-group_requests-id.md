<!-- --- title: DELETE /group_requests/:id -->

This allows the recipient of a group request to delete the invite. The sender of the request is not allowed to delete the request, only the recipient. Deletion of the request is the action taken when the group owner rejects the requests.

=
####Authentication:
The user needs to be logged in and have valid credentials to use this route.

=
####Parameters:
:group_requests_id - Integer, passed in the URL. Is derived from the 'id' field on the 'group_requests' table.

=
####API request example:
```json
http://stage-api-access.evant.com/group_requests/234
```

=
####JSON response example:

[[include:/json/JSON_NO_RESPONSE]]

This requests provides a <strong>HTML 204</strong> on success.