<!-- --- title: GET /messages/user_search/:query -->

This is route to search for other users that the active user are able to message. The actual functionality of the search function is still under development, but the general methodology of this route should remain fairly static.

=
####Authentication:

The user needs to be logged in and have valid credentials to use this route.

=
####Parameters:

:query, simple text passed in

=
####Response:

This requests provides a <strong>HTML 200</strong> on success.

=
####API request example:
```html
http://example.com/messages/user_search/b
```

=
####JSON response example:

[[include:/json/JSON_NEEDS_EXAMPLE]]

=
####Response Data Detail:

[[include:/serializers/user_nano]]