<!-- --- title: PUT /user_connections/:id -->

Changes a user_connection request to being approved. There is a field 'is_approved' on the 'user_connections' table that is the value that gets changed. This field has a default boolean value of 0, which gets changed to 1 after this route has been run.

=
#### Authentication

The user needs to be logged in and have valid credentials to use this route.

=
#### Parameters

:user_connection_id - Integer, passed in through the URL. Is derived from the 'id' field on the 'user_connection' table.

=
####API request example:
```json
http://stage-api-access.evant.com//user_connections/159
```

=
####JSON response example:

```json
{"user_connection"=>
  {"id"=>159,
   "body"=>"I'd like to connect",
   "is_approved"=>true,
   "sender_user_id"=>12606,
   "recipient_user_id"=>12603,
   "SenderUser"=>
    {"id"=>12606,
     "first_name"=>"Mustafa",
     "last_name"=>"Schinner",
     "title"=>"Random User",
     "organization_name"=>"Gorczany-Morar",
     "photo"=>
      "https://assets.evanta.com/shared/resources/Users/large/anonymous2.jpg",
     "user_role_id"=>12608},
   "RecipientUser"=>
    {"id"=>12603,
     "first_name"=>"Generic",
     "last_name"=>"User",
     "title"=>"CEO of QA",
     "organization_name"=>"Evanta",
     "photo"=>
      "https://assets.evanta.com/shared/resources/Users/large/anonymous2.jpg",
     "user_role_id"=>12607}}}
```

This requests provides a <strong>HTML 201</strong> on success.