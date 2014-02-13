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
  {"id"=>1772,
   "unread"=>false,
   "viewed_date"=>nil,
   "body"=>
    "[\"Rerum maxime alias et nihil repellat. Recusandae est id. Rerum possimus aut eum voluptatum sed quibusdam cum. Quia nihil repudiandae. Magnam soluta temporibus unde.\"]",
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