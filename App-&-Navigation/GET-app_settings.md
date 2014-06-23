<!-- --- title: GET /app_settings -->

This route returns a boolean value on the current status of an app setting as it relates to the active user. The app_settings route is the odd duck of this project. There are a number of different text parameters that can be passed in, and some of those text parameters can then be further modified by appending those text paramters with either group_ids or event_ids. The ability to do this is not indicated anywhere.

It is possible to pass in more than one app_setting parameter at a time. Each app_setting can only have one additional parameter (event or group) passed in. The app_settings should be seperated by an ampersand '&'.


=
####Authentication:

The user needs to be logged in and have valid credentials to use this route.

=
####Parameters:

| name | description | type |
|------|-------------|------|
| :group_id | Is derived from the 'id' field on the 'groups' table. | integer
| :event_id | Is derived from the 'id' field on the 'events' table. | integer
| app_setting_key| A string key passed in that references an app_setting | string

=
####Response:

This requests provides a <strong>HTML 200</strong> on success.

=
####API request example:
```html
http://example.com/app_settings/?names[]=event_follows&event_id=#{event.id}

http://example.com/app_settings/?names[]=support_link&names[]=send_messages&names[]=groups_in_navigation&names[]=show_me_on_lists&names[]=like_posts&names[]=show_group_member_list&names[]=post_comment_updates&names[]=delete_post_warning&names[]=event_session_evaluations&group_id=#{group.id}&event_id=#{event.id}

```

=
####List of app_setting keys:

Some of these keys appear twice in the list, with and without an additional parameter. If that key is passed in without a paramter, it will return a value from the application level. If passed in with the parameter, it will be specifically for inside of that group or event.

[[include:/post_data/app_settings_parameters]]