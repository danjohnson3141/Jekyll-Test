<!-- --- title: GET /user_connections/pending -->

Returns a list of **all** user_connection records that currently have 'is_approved' as 'false'. This returns records where the active user is either the sender or recipeint of the connection request.

=
####Authentication:

The user needs to be logged in and have valid credentials to use this route.

=
####Parameters:

none; defaults only

=
####Response:

This requests provides a <strong>HTML 200</strong> on success.

=
####API request example:
```html
http://example.com/user_connections/pending
```

=
####JSON response example:

An array of user_connection objects

[[include:/json/JSON_GET_user_connections_pending]]

=
####Response Data Detail:

[[include:/serializers/user_connection]]