<!-- --- title: GET /users/profile/:id -->

This brings back **one** user's profile.

=
#### Authentication

The user needs to be logged in and have valid credentials to use this route.

=
#### Parameters

:user_id - Integer, passed in through the URL. Is derived from the 'id' field on the 'users' table. This the profile that will be returned.

=
####JSON request example:
```
http://0.0.0.0:3000/users/profile/18447
```

=
####JSON response example:

```json
{"user"=>
  {"id"=>18447,
   "email"=>"tamara.hodkiewicz@mcdermott.net",
   "alt_email"=>"sylvester.considine@gmail.com",
   "first_name"=>"Brenden",
   "last_name"=>"Beatty",
   "title"=>"Random User",
   "organization_name"=>"Murphy, O'Kon and Connelly",
   "bio"=>
    "Illum sed dolores temporibus est sit et aut consectetur sit inventore.",
   "photo"=>
    "https://assets.evanta.com/shared/resources/Users/large/anonymous2.jpg",
   "user_role_id"=>18449,
   "user_connection_id"=>nil}}
```

This requests provides a <strong>HTML 200</strong> on success.