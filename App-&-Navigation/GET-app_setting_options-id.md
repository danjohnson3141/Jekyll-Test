<!-- --- title: GET /app_setting_options/:id -->

This route returns info on an app setting and what other app settings its dependent on, this route is for debugging and not publiclly facing.

=
####Authentication:

The user needs to be logged in and have valid credentials to use this route.

=
####Parameters:

:id - integer - 

=
####Response:

This requests provides a <strong>HTML 200</strong> on success.

=
####API request example:
```html
http://example.com/app_setting_options/3

=
####JSON response example:

[[include:/json/JSON_GET_app_setting_options_id]]

=
####Response Data Detail:

[[include:/serializers/app_setting_option_user]]