<!-- --- title: GET /users/locale_options -->

Returns a list of possible language preferences for the active user to select from while editing their profile. This will affect the labels being passed in through the API and at some point will also affect how numbers, dates and times are displayed. However, much of this functionality is still in development.

=
####Authentication:

The user needs to be logged in and have valid credentials to use this route.

=
####Parameters:

LIST OF ALL PARAMETERS AND WHAT THEY ARE

=
####Response:

This requests provides a <strong>HTML 200</strong> on success.

=
####API request example:
```html
http://example.com/users/locale_options
```

=
####JSON response example:

[[include:/json/JSON_GET_users_locale_options]]

=
####Response Data Detail:

[[include:/serializers/EXAMPLE]]