Returns the active users's profile.

=
#### Authentication

The user needs to be logged in and have valid credentials to use this route.

=
#### Parameters

none; defaults only

=
####JSON request example:
```
http://0.0.0.0:3000/users/profile
```

=
####JSON response example:

```
{"user"=>
  {"id"=>19845,
   "email"=>"generic_user@evanta.com",
   "alt_email"=>nil,
   "first_name"=>"Generic",
   "last_name"=>"User",
   "title"=>"CEO of QA",
   "organization_name"=>"Evanta",
   "bio"=>"This is the biography of the default Generic User",
   "photo"=>
    "https://assets.evanta.com/shared/resources/Users/large/anonymous2.jpg",
   "user_role_id"=>19849,
   "user_connection_id"=>nil}}
```

This requests provides a <strong>HTML RESPONSE NUMBER</strong> on success.