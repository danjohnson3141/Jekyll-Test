<!-- --- title: PUT /group_requests/:id -->

This is the method by which a group owner is able to approve the request of a different owner who requested to join that group. The group owner is unable to unapprove the group request once it's been approved. 

=
####Authentication:

The user needs to be logged in and have valid credentials to use this route.

=
####Parameters:

(group_requests) :id - Integer, passed in the URL. Is derived from the 'id' field on the 'group_requests' table.

=
####Response:

This requests provides a <strong>HTML 204</strong> on success.

=
####API request example:
```json
http://stage-api-access.evant.com/group_requests/234
```

=
####Post Data:
{ group_request: {is_approved: true} }


=
####JSON response example:

[[include:/json/JSON_NO_RESPONSE]]