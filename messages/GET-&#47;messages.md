<!-- --- title: GET /messages -->

This route gets the inbox messages view for the logged in user. The 'inbox view' returns only the most recent conversation threads with each person the user was communicating with.

=
#### Authentication
The user needs to be logged in and have valid credentials to use this route.

=
#### Parameters
none; only default response

=
####JSON request example:
```
http://0.0.0.0:3000/messages
```

=
####JSON response example:

```json
{"messages"=>
  [{"id"=>1105,
    "unread"=>true,
    "viewed_date"=>nil,
    "body"=>"Sharable client-server archive",
    "sender_user_id"=>12638,
    "recipient_user_id"=>12637,
    "created_at"=>"2014-02-12T15:58:27.000Z",
    "ago"=>"1d",
    "user"=>
     {"id"=>12638,
      "first_name"=>"Albina",
      "last_name"=>"Durgan",
      "title"=>"Random User",
      "organization_name"=>"Reichel-Deckow",
      "photo"=>nil,
      "user_role_id"=>nil,
      "user_connection_id"=>nil}},
   {"id"=>1106,
    "unread"=>false,
    "viewed_date"=>"2014-02-11T15:58:27.000Z",
    "body"=>"Open-architected next generation local area network",
    "sender_user_id"=>12639,
    "recipient_user_id"=>12637,
    "created_at"=>"2014-02-10T15:58:27.000Z",
    "ago"=>"3d",
    "user"=>
     {"id"=>12639,
      "first_name"=>"Malvina",
      "last_name"=>"Carter",
      "title"=>"Random User",
      "organization_name"=>"Olson and Sons",
      "photo"=>nil,
      "user_role_id"=>nil,
      "user_connection_id"=>nil}}]}
 
```

This requests provides a <strong>HTML 200</strong> on success.