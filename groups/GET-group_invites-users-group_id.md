<!-- --- title: GET /group_invites/users/:group_id -->

Returns all of the pending user invites for a group. Should not return any invites for users who members of the group. Should only return any values if the user is the owner of the group.

=
#### Authentication

The user needs to be logged in and have valid credentials to use this route.

=
#### Parameters

:group_id - Integer, passed in through the URL. Is derived from the 'id' field on the 'groups' table.

=
####JSON request example:
```json
http://stage-api-access.evant.com/group_invites/users/1158
```

=
####JSON response example:

```json
{"group_invites"=>
  [{"id"=>176,
    "group_id"=>1158,
    "user"=>
     {"id"=>9666,
      "email"=>"felicita.beahan@beer.info",
      "alt_email"=>"landen@hotmail.com",
      "first_name"=>"Dorcas",
      "last_name"=>"Zemlak",
      "title"=>"Random User",
      "organization_name"=>"Brown Group",
      "bio"=>"Est blanditiis a in quo ex voluptatem ratione velit itaque.",
      "photo"=>
       "https://assets.evanta.com/shared/resources/Users/large/anonymous.jpg",
      "user_role_id"=>9668,
      "user_connection_id"=>nil}},
   {"id"=>175,
    "group_id"=>1158,
    "user"=>
     {"id"=>9663,
      "email"=>"gregorio_smith@moenheathcote.net",
      "alt_email"=>"timothy@hotmail.com",
      "first_name"=>"Fannie",
      "last_name"=>"Simonis",
      "title"=>"Random User",
      "organization_name"=>"Gleason, Hettinger and Larkin",
      "bio"=>
       "Ut et et modi qui et consequatur iure nihil impedit fugiat accusantium sit.",
      "photo"=>
       "https://assets.evanta.com/shared/resources/Users/large/anonymous.jpg",
      "user_role_id"=>9665,
      "user_connection_id"=>nil}}]}
```

This requests provides a <strong>HTML 200</strong> on success.