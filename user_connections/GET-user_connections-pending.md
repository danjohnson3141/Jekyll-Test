<!-- --- title: GET /user_connections/pending -->

Returns a list of **all** user_connection records that currently have 'is_approved' as 'false'.

=
#### Authentication

The user needs to be logged in and have valid credentials to use this route.

=
#### Parameters

none; defaults only

=
####API request example:
```json
http://stage-api-access.evant.com/user_connections/pending
```

=
####JSON response example:

```json
{"user_connections"=>
  [{"id"=>144,
    "is_approved"=>false,
    "is_approver"=>false,
    "user"=>
     {"id"=>8938,
      "first_name"=>"Gonzalo",
      "last_name"=>"Volkman",
      "title"=>"Random User",
      "organization_name"=>"O'Connell LLC",
      "photo"=>
       "https://assets.evanta.com/shared/resources/Users/large/anonymous2.jpg"}},
   {"id"=>145,
    "is_approved"=>false,
    "is_approver"=>true,
    "user"=>
     {"id"=>8939,
      "first_name"=>"Jarod",
      "last_name"=>"McClure",
      "title"=>"Random User",
      "organization_name"=>"Jast, Bergnaum and DuBuque",
      "photo"=>
       "https://assets.evanta.com/shared/resources/Users/large/anonymous2.jpg"}}]}
```

This requests provides a <strong>HTML 200</strong> on success.