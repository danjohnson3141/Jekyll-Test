<!-- --- title: GET /messages -->

This route gets the inbox messages view for the logged in user. The 'inbox view' returns only the single most recent with each person the user was communicating with.

=
####Authentication:
The user needs to be logged in and have valid credentials to use this route.

=
####Parameters:
none; only default response

=
####Response:

This requests provides a <strong>HTML 200</strong> on success.

=
####API request example:
```html
http://example.com/messages
```

=
####JSON response example:

This route returns an array of message objects.

[[include:/json/JSON_GET_messages]]

=
####Response Data Detail

[[include:/serializers/message]]