<!-- --- title: GET /messages -->

This route gets the inbox messages view for the logged in user. The 'inbox view' returns only the most recent conversation threads with each person the user was communicating with. This route returns an array of message objects.

=
####Authentication:
The user needs to be logged in and have valid credentials to use this route.

=
####Parameters:
none; only default response

=
####API request example:
```json
http://stage-api-access.evant.com/messages
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
=
####Response Data Detail

| name              | description                                      | type    |
|-------------------|--------------------------------------------------|---------|
| id                | the id of the message being returned             | integer |
| unread            | whether the message has been read yet            | boolean |
| viewed_date       | the date that the message was viewed             | string  |
| body              | content of the message                           | string  |
| sender_user_id    | the id of the user that sent the message         | integer |
| recipient_user_id | the id of the the user that received the message | integer |
| created_at        | when the message was created                     | string  |
| ago               | how long ago the message was created             | string  |

This requests provides a <strong>HTML 200</strong> on success.