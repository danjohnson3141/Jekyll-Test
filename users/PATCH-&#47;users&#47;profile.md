<!-- --- title: PATCH /users/profile -->

This is the route that allows the active user to alter their profile.

=
#### Authentication

The user needs to be logged in and have valid credentials to use this route.

=
#### Parameters

:alt_email - Varchar, passed in through the post data. Is derived from the 'alt_email' field on the 'users' table.

:bio  - Text, passed in through the post data. Is derived from the 'bio' field on the 'users' table. 

:first_name - Varchar, passed in through the post data. Is derived from the 'first_name' field on the 'users' table.

:last_name - Varchar, passed in through the post data. Is derived from the 'last_name' field on the 'users' table.

:organization_name - Varchar, passed in through the post data. Is derived from the 'organization_name' field on the 'users' table. 

:photo - Varchar, passed in through the post data. Is derived from the 'photo' field on the 'users' table.

:title - Varchar, passed in through the post data. Is derived from the 'title' field on the 'users' table.

=
####JSON request example:
```json
http://0.0.0.0:3000/users/profile
```

=
####Post Data
```
{ user: 
  { alt_email: "alt@example.com", 
    bio: "I'm totally awesome!!", 
    first_name: "Awesome", 
    last_name: "UserTest", 
    organization_name: "Testing is awesome!", 
    photo: "www.example.com/updated.gif", 
    title: "King of the World" }
 }
```

=
####JSON response example:

```json
none; default only
```

This requests provides a <strong>HTML 204</strong> on success.