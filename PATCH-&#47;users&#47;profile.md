This is the route that allows the active user to alter their profile.

=
#### Authentication

Declare what authentications are required

Good sample text: The user needs to be logged in and have valid credentials to use this route.

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
```
http://0.0.0.0:3000/users/profile
```

=
####Post Data
```

```

=
####JSON response example:

```
none; default only
```

This requests provides a <strong>HTML 204</strong> on success.