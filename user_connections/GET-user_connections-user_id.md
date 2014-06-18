<!-- --- title: GET /user_connections/user/:user_id -->

Returns a list of all the visible user connections that a user has. 

=
####Authentication:

The user needs to be logged in and have valid credentials to use this route.

=
####Parameters:

:user_id - Integer, passed in through the URL. Is derived from the 'id' field on the 'users' table. This returns connections where the user is either the recipient or the sender.

=
####Response:

This requests provides a <strong>HTML 200</strong> on success.

=
####API request example:
```html
http://example.com/users/connections/17065
```

=
####JSON response example:

An array of user_connection objects

[[include:/json/JSON_GET_user_connections_user_user_id]]

=
####Response Data Detail:

[[include:/serializers/user_connection]]