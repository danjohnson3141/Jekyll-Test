<!-- --- title: GET /app_settings -->

This route returns a boolean value on the current status of an app setting as it relates to the active user. The app_settings route is the odd duck of this project. There are a number of different text parameters that can be passed in, and some of those text parameters can then be further modified by appending those text paramters with either group_ids or event_ids. The ability to do this is not indicated anywhere.

It is possible to pass in more than one app_setting parameter at a time. Each app_setting can only have one additional parameter (event or group) passed in. The app_settings should be seperated by an ampersand '&'.


=
####Authentication:

The user needs to be logged in and have valid credentials to use this route.

=
####Parameters:

| name | description | type |
-----------------------------
| :group_id | Is derived from the 'id' field on the 'groups' table. | integer
| :event_id | Is derived from the 'id' field on the 'events' table. | integer
| app_setting_key| A string key passed in that references an app_setting | string

=
####Response:

This requests provides a <strong>HTML 200</strong> on success.

=
####API request example:
```html
http://example.com/app_settings
```

=
####List of app_setting keys:

[[include:/post_data/app_settings_parameters]]