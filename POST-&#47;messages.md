This is the route for creating a new message, being sent from the logged in user to another user. The sender_user_id is set from the

=
#### Authentication
The user needs to be logged in and have valid credentials to use this route.

=
#### Parameters
:body, this is the actual text of the message being sent

:recipient_user_id, this is 'user_id' of the person that is receiving the message

=
####JSON request example:
```
http://0.0.0.0:3000/messages
```

=
####Post Data
```
{ message: {body: "THIS TEXT COMPOSES THE BODY OF THE MESSAGE", recipient_user_id: 2345} }
```
=
####JSON response example:

```
{"message"=>
  {"id"=>1735,
   "unread"=>true,
   "viewed_date"=>nil,
   "body"=>
    "[\"THIS TEXT COMPOSES THE BODY OF THE MESSAGE\"]",
   "sender_user_id"=>15,
   "recipient_user_id"=>2345,
   "created_at"=>"2014-02-13T23:06:47.997Z",
   "ago"=>"0m",
   "user"=>
    {"id"=>15,
     "first_name"=>"Generic",
     "last_name"=>"User",
     "title"=>nil,
     "organization_name"=>nil,
     "photo"=>nil,
     "user_role_id"=>nil,
     "user_connection_id"=>nil}}}
```

This requests provides a <strong>HTML RESPONSE NUMBER</strong> on success.