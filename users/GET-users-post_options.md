<!-- --- title: GET /users/post_options -->

Returns a list of groups and events that the user is able to create posts for. This is used by the app when creating a post from the user feed rather than from inside the respective groups or events.

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
http://example.com/users/post_options
```

=
####JSON response example:

[[include:/json/JSON_GET_users_post_options]]

=
####Response Data Detail:

[[include:/serializers/user_post_option]]