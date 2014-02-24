PLAIN ENGLISH DESCRIPTION OF THE ROUTE

=
#### Authentication

Declare what authentications are required

Good sample text: The user needs to be logged in and have valid credentials to use this route.

=
#### Parameters

LIST OF ALL PARAMETERS AND WHAT THEY ARE

=
####JSON request example:
```
http://0.0.0.0:3000/ROUTE_NAME
```

=
####Post Data
```
{ user: 
  { reset_password_token: "S8cL7iZCLrX3WURW2vaN",  
    password: "evanta2015", 
    password_confirmation: "evanta2015" } 
  }
```

=
####JSON response example:

```
NO JSON RESPONSE
```

This requests provides a <strong>HTML 200</strong> on success.