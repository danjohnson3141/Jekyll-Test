<!-- --- title: GET /users/industry_type_options -->

Returns a list of **all** the industry types that the active user is able to choose from while editing their profile.

=
####Authentication: 

The user needs to be logged in and have valid credentials to use this route.

=
####Parameters:

None; default only.

=
####Response:

This requests provides a <strong>HTML 200</strong> on success.

=
####API request example:
```html
http://example.com/users/industry_type_options
```

=
####JSON response example:

[[include:/json/JSON_GET_users_industry_type_options]]

=
####Response Data Detail:

[[include:/serializers/industry_type]]