<!-- --- title: PUT /users/password -->

This is how the user resets their password. They need to have a 'reset_password_token' which is sent to them via their email address. After they've received this token, they're able to update their password, which is then encrypted (and salted? I don't know) and stored in the 'encrypted_password' field of the 'users' table.

=
####Authentication:

The active user does not need to be logged in for this route to work.

=
####Parameters:

:password - Passed in through the post data. This is the users new password. Is not stored in plaintext anywhere.

:password_confirmation - Passed in through the post data. This is used to verify that the new user has entered the correct updated password by having them submit it twice and

:reset_password_token - Varchar, passed in through the post data. This is derived from the 'reset_password_token' field on the 'users' table.

=
####API request example:
```html
http://example.com/users/password
```

=
####Post data example:
```
{ user: 
  { reset_password_token: "S8cL7iZCLrX3WURW2vaN",  
    password: "evanta2015", 
    password_confirmation: "evanta2015" } 
 }
```

=
####JSON response example:

[[include:/json/JSON_NO_RESPONSE]]

This requests provides a <strong>HTML 200</strong> on success.