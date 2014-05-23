<!-- --- title: POST /messages -->

This is the route for creating a new message, being sent from the logged in user to another user. The sender_user_id is set from the

=
####Authentication:
The user needs to be logged in and have valid credentials to use this route.

=
####Parameters:
:body - Text, passed in through the post data. This is the plain text of the submission.

:recipient_user_id - Integer, passed in through the post data. This is 'user_id' of the person that is receiving the message. Derived from the 'id' field of the 'users' table'.

=
####Response:

This requests provides a <strong>HTML 201</strong> on success.

=
####API request example:
```html
http://example.com:3000/messages
```

=
####Post data example:
```
{ message: 
  {body: "THIS TEXT COMPOSES THE BODY OF THE MESSAGE", 
   recipient_user_id: 2345} 
 }
```
=
###Post data detail:

[[include:/post_data/post_messages]]

=
####JSON response example:

[[include:/json/JSON_POST_messages]]

=
####Response Data Detail:

[[include:/serializers/message]]