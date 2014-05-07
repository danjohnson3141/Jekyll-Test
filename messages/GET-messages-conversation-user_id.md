<!-- --- title: GET /messages/conversation/:user_id -->

Requests all of the non-archived messages between the logged in user and a second party. The ':user_id' parameter looks at both the 'sender_user_id' and 'recipient_user_id' fields from the 'messages' table. 

=
#### Authentication

The user needs to be logged in and have valid credentials to use this route.

=
#### Parameters

:user_id - Integer, passed in through the URL. Is derived from the 'id' field on the 'users' table. 

=
####JSON request example:
```json
http://stage-api-access.evant.com/messages/conversation/18655
```

=
####JSON response example:

```json
{"messages"=>
  [{"id"=>1624,
    "unread"=>false,
    "viewed_date"=>nil,
    "body"=>"Enhanced holistic Graphic Interface",
    "sender_user_id"=>18655,
    "recipient_user_id"=>18656,
    "created_at"=>"2014-02-13T22:26:01.000Z",
    "ago"=>"0m"},
   {"id"=>1625,
    "unread"=>false,
    "viewed_date"=>"2014-02-13T22:26:07.000Z",
    "body"=>"Pre-emptive intangible support",
    "sender_user_id"=>18656,
    "recipient_user_id"=>18655,
    "created_at"=>"2014-02-13T22:26:01.000Z",
    "ago"=>"0m"},
   {"id"=>1626,
    "unread"=>false,
    "viewed_date"=>nil,
    "body"=>"Distributed modular definition",
    "sender_user_id"=>18655,
    "recipient_user_id"=>18656,
    "created_at"=>"2014-02-13T22:26:01.000Z",
    "ago"=>"0m"}]}
```

This requests provides a <strong>HTML 200</strong> on success.