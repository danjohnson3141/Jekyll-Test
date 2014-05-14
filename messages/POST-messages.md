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
####API request example:
```json
http://example.com:3000/messages
```

=
####Post Data:
```
{ message: 
  {body: "THIS TEXT COMPOSES THE BODY OF THE MESSAGE", 
   recipient_user_id: 2345} 
 }
```
=
####JSON response example:

```json
{"message"=>
  {"id"=>1772,
   "unread"=>false,
   "viewed_date"=>nil,
   "body"=>
    "[\"THIS TEXT COMPOSES THE BODY OF THE MESSAGE\"]",
   "sender_user_id"=>15,
   "recipient_user_id"=>2345,
   "created_at"=>"2014-02-13T23:12:01.350Z",
   "ago"=>"0m",
   "user"=>
    {"id"=>2345,
     "first_name"=>"Brandyn",
     "last_name"=>"Parker",
     "title"=>"Random User",
     "organization_name"=>"Schneider LLC",
     "photo"=>nil,
     "user_role_id"=>nil,
     "user_connection_id"=>nil}}}
```

This requests provides a <strong>HTML 200</strong> on success.