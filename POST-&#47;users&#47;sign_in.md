PLAIN ENGLISH DESCRIPTION OF THE ROUTE

=
#### Authentication

Declare what authentications are required

Good sample text: The user needs to be logged in and have valid credentials to use this route.

=
#### Parameters

:email - Varchar, passed in through the post data. Is derived from the 'email' field on the 'users' table.

:password - Varchar, passed in through the post data. Is compared against the 'encrypted_password' field on the 'users' table.


=
####Post Data
```
{ user: 
  { email: "generic_user@evanta.com", 
    password: "evanta2014"} 
 }
```

=
####JSON request example:
```
http://0.0.0.0:3000/ROUTE_NAME
```

=
####JSON response example:

```
{"success"=>true, "auth_token"=>"54321"}
```

This requests provides a <strong>HTML 200</strong> on success.