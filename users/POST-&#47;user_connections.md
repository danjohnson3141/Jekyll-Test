<!-- --- title: POST /user_connections -->

This is how the active user submits a new user connection request.

=
#### Authentication

The user needs to be logged in and have valid credentials to use this route.

=
#### Parameters

:body - Text, passed in through the post data. This is the plain text of the submission.

:recipient_user_id - Integer, passed in through the post data. This is 'user_id' of the person that is receiving the message. Derived from the 'id' field of the 'users' table'.

:sender_user_id - Integer, passed in through the post data. This is 'user_id' of the person that is receiving the message. Derived from the 'id' field of the 'users' table'.

=
####JSON request example:
```json
http://0.0.0.0:3000/user_connections
```

=
####JSON response example:

```json
{"user_connection"=>
  {"id"=>151,
   "body"=>"I'd like to connect",
   "is_approved"=>false,
   "sender_user_id"=>12018,
   "recipient_user_id"=>12021,
   "SenderUser"=>
    {"id"=>12018,
     "first_name"=>"Generic",
     "last_name"=>"User",
     "title"=>"CEO of QA",
     "organization_name"=>"Evanta",
     "photo"=>
      "https://assets.evanta.com/shared/resources/Users/large/anonymous2.jpg",
     "user_role_id"=>12022},
   "RecipientUser"=>
    {"id"=>12021,
     "first_name"=>"Cloyd",
     "last_name"=>"Muller",
     "title"=>"Random User",
     "organization_name"=>"McDermott, Renner and McCullough",
     "photo"=>
      "https://assets.evanta.com/shared/resources/Users/large/anonymous2.jpg",
     "user_role_id"=>12023}}}
```

This requests provides a <strong>HTML 201</strong> on success.