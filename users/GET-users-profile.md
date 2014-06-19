<!-- --- title: GET /users/profile -->

Returns the active user's profile. Not to be confused with the /users/profile/:user_id route.

=
####Authentication:

The user needs to be logged in and have valid credentials to use this route.

=
####Parameters:

None; default only

=
####Response:

This requests provides a <strong>HTML 200</strong> on success.

=
####API request example:
```html
http://example.com/users/profile
```

=
####JSON response example:

[[include:/json/JSON_GET_users_profile]]

=
####Response Data Detail:

[[include:/serializers/user]]