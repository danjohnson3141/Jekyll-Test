<!-- --- title: PUT /user_connections/:id -->

Changes a user_connection request to being approved. There is a field 'is_approved' on the 'user_connections' table that is the value that gets changed. This field has a default boolean value of 0, which gets changed to 1 after this route has been run. The user is only able to PATCH records where they are the connection recipient. No post data is passed in with this route. If the record is already approved and this is attempted, they should receive a 422 error.

=
####Authentication:

The user needs to be logged in and have valid credentials to use this route.

=
####Parameters:

:id - Integer, passed in through the URL. Is derived from the 'id' field on the 'user_connection' table.

=
####Response:

This requests provides a <strong>HTML 201</strong> on success.

=
####API request example:
```html
http://stage-api-access.evant.com/user_connections/159
```

=
####Post data example:
```
NO POST DATA USED
```

=
####JSON response example:

[[include:/json/JSON_NO_RESPONSE]]