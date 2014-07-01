<!-- --- title: GET /users/profile/:user_id -->

Returns the user profile for the user indicated in the parameter

=
####Authentication:

The user needs to be logged in and have valid credentials to use this route.

=
####Parameters:

:user_id - Integer, passed in through the URL. Is derived from the 'id' field on the 'users' table.

=
####Response:

This requests provides a <strong>HTML 200</strong> on success.

=
####API request example:
```html
http://example.com/users/profile/4
```

=
####JSON response example:

[[include:/json/JSON_GET_users_profile_user_id]]

=
####Response Data Detail:

[[include:/serializers/user]]