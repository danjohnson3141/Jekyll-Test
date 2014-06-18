<!-- --- title: GET /users/region_options -->

Returns a list of of regions available for the user to select from. This is then displayed on the user's profile.

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
http://example.com/users/region_options
```

=
####JSON response example:

returns an array of region objects

[[include:/json/JSON_GET_users_region_options]]

=
####Response Data Detail:

[[include:/serializers/region]]