<!-- --- title: POST /user_connections -->

This is how the active user submits a new user connection request. The request is created with a default value of 0 (or false) in the ```is_approved``` field. The intended recipient of the connection is one that edits the record to having a value of 1 (or true) in that field.

=
####Authentication:

The user needs to be logged in and have valid credentials to use this route.

=
####Parameters:

None; default only.

=
####Response:

This requests provides a <strong>HTML 201</strong> on success.

=
####API request example:
```json
http://stage-api-access.evant.com/user_connections
```

=
####Post data example:
```
{ user_connection: 
  { recipient_user_id: 5 } }
```
 
=
###Post data detail:

[[include:/post_data/post_user_connections]]

=
####JSON response example:

[[include:/json/JSON_POST_user_connections]]

=
####Response Data Detail:

[[include:/serializers/user_connection]]