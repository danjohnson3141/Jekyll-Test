<!-- --- title: GET /messages/conversation/:user_id -->

Requests all of the non-archived messages between the logged in user and a second party. The ':user_id' parameter looks at both the 'sender_user_id' and 'recipient_user_id' fields from the 'messages' table. 

=
####Authentication:

The user needs to be logged in and have valid credentials to use this route.

=
####Parameters:

:user_id - Integer, passed in through the URL. Is derived from the 'id' field on the 'users' table. 

=
####Response:

This requests provides a <strong>HTML 200</strong> on success.

=
####API request example:
```html
http://example.com/messages/conversation/18655
```

=
####JSON response example:

Returns an array of message objects

[[include:/json/JSON_GET_messages_conversation_user_id]] 

=
####Response Data Detail:


[[include:/serializers/message]]