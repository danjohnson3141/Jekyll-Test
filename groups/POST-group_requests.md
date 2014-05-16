<!-- --- title: POST /group_requests -->

This creates a new record for the user trying to join a group that requires approval to join.

=
####Authentication:

The user needs to be logged in and have valid credentials to use this route.

=
####Parameters:

:group_id - Integer, passed in through the post data. Is derived from the 'id' field on the 'groups' table. This is the group that the user is requesting to join.

:user_id - Integer, passed in through the post data. Derived from the 'id' field of the 'users' table.

=
####Response:

This requests provides a <strong>HTML 201</strong> on success.

=
####API request example:
```json
http://stage-api-access.evant.com/group_requests
```

=
####Post data example:
```
{ group_request: 
  { group_id: 706 } 
 }
```

=
###Post data detail:

[[include:/post_data/post_group_request]]

=
####JSON response example:

[[include:/json/JSON_POST_group_request]]

=
####Response Data Detail:

[[include:/serializers/group_request]]