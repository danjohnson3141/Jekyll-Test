<!-- --- title: GET /app_setting_options/:id -->

Returns information on specific app_setting options, most specifically any dependencies that app_setting may have. This is a development tool and isn't actually part of the app itself.

=
####Authentication:

The user needs to be logged in and have valid credentials to use this route.

=
####Parameters:

:id (app_setting_option) - Integer, passed in the URL. Is derived from the 'id' field on the the 'app_setting_option' table.

=
####Response:

This requests provides a <strong>HTML 200</strong> on success.

=
####API request example:
```html
http://example.com/app_setting_options/text
```

=
####JSON response example:

[[include:/json/JSON_GET_app_setting_options_id]]

=
####Response Data Detail:

[[include:/serializers/EXAMPLE]]