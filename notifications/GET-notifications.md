<!-- --- title: GET /notifications -->

Returns **all** of the notifications for the active user.

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
http://example.com/notifications
```

=
####JSON response example:

[[include:/json/JSON_GET_notifications]]

=
####Response Data Detail:

[[include:/serializers/notification]]