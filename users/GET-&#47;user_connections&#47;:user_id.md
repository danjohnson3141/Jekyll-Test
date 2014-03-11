<!-- --- title: GET /user_connections/:user_id -->

Returns a list of all the user connections that a user has. 

=
#### Authentication

The user needs to be logged in and have valid credentials to use this route.

=
#### Parameters

:user_id - Integer, passed in through the URL. Is derived from the 'id' field on the 'users' table. This returns connections where the user is either the recipient or the sender.

=
####JSON request example:
```
http://0.0.0.0:3000/user_connections/17065
```

=
####JSON response example:

```json
{"user_connections"=>
  [{"id"=>320,
    "body"=>"Connect1",
    "is_approved"=>true,
    "sender_user_id"=>17065,
    "recipient_user_id"=>17068,
    "SenderUser"=>
     {"id"=>17065,
      "first_name"=>"Laron",
      "last_name"=>"Friesen",
      "title"=>"Random User",
      "organization_name"=>"Hand, Kuhn and Williamson",
      "photo"=>
       "https://assets.evanta.com/shared/resources/Users/large/anonymous2.jpg",
      "user_role_id"=>17067},
    "RecipientUser"=>
     {"id"=>17068,
      "first_name"=>"Ophelia",
      "last_name"=>"Rowe",
      "title"=>"Random User",
      "organization_name"=>"Volkman-Nikolaus",
      "photo"=>
       "https://assets.evanta.com/shared/resources/Users/large/anonymous2.jpg",
      "user_role_id"=>17070}},
   {"id"=>321,
    "body"=>"Connect2",
    "is_approved"=>true,
    "sender_user_id"=>17071,
    "recipient_user_id"=>17065,
    "SenderUser"=>
     {"id"=>17071,
      "first_name"=>"Kimberly",
      "last_name"=>"Bergstrom",
      "title"=>"Random User",
      "organization_name"=>"Block and Sons",
      "photo"=>
       "https://assets.evanta.com/shared/resources/Users/large/anonymous2.jpg",
      "user_role_id"=>17073},
    "RecipientUser"=>
     {"id"=>17065,
      "first_name"=>"Laron",
      "last_name"=>"Friesen",
      "title"=>"Random User",
      "organization_name"=>"Hand, Kuhn and Williamson",
      "photo"=>
       "https://assets.evanta.com/shared/resources/Users/large/anonymous2.jpg",
      "user_role_id"=>17067}}]}
```

This requests provides a <strong>HTML 200</strong> on success.