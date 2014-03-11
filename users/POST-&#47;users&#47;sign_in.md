<!-- --- title: POST /users/sign_in -->

This is the route that the user uses to login.

=
#### Authentication

The user does not need to be logged in to use this route.

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
```json
http://0.0.0.0:3000/users/sign_in
```

=
####JSON response example:

```json
{"success"=>true, "auth_token"=>"54321"}
```

This requests provides a <strong>HTML 200</strong> on success.