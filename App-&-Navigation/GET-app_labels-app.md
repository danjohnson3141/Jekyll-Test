<!-- --- title: GET /app_labels/app -->

This route returns a list of all the text that will be used by the app. The text being returned can be affected the the language settings of the user.

=
####Authentication:

Good sample text: The user needs to be logged in and have valid credentials to use this route.

=
####Parameters:

none; default only

=
####Response:

This requests provides a <strong>HTML 200</strong> on success.

=
####API request example:
```html
http://example.com/app_labels/app
```
 
=
####JSON response example:

[[include:/json/JSON_GET_app_labels_app]]

=
####Response Data Detail:

[[include:/serializers/app_label]]