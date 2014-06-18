<!-- --- title: GET /users/settings -->

Returns a list of user modifiable settings for the app. This is broken up into two types, `Preferences` and `Privacy` those can then be subdivided based on the category.

=
####Authentication:

The user needs to be logged in and have valid credentials to use this route.

=
####Parameters:

None; default ony.

=
####Response:

This requests provides a <strong>HTML 200</strong> on success.

=
####API request example:
```html
http://example.com/users/settings
```

=
####JSON response example:

[[include:/json/JSON_GET_users_settings]]

=
####Response Data Detail:

[[include:/serializers/app_setting_option_user]]