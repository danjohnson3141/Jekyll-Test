<!-- --- title: POST /users/sign_in -->

This is the route that the active user uses to login. After a succseful login, the app provides the active user with an authorization token that will be needed in order to use most other routes within the application. 

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
####API request example:
```json
http://stage-api-access.evant.com/users/sign_in
```

=
####JSON response example:

```json
{"success"=>true, "auth_token"=>"54321"}
```

This requests provides a <strong>HTML 200</strong> on success.