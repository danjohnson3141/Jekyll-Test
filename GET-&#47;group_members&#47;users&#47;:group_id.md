Returns a list of all of the members of a group.

=
#### Authentication

The user needs to be logged in and have valid credentials to use this route.

=
#### Parameters

:group_id - Integer, passed in through the URL. Is derived from the 'id' field on the 'groups' table.

=
####JSON request example:
```
http://0.0.0.0:3000/group_members/users/1671
```

=
####JSON response example:

```
{"group_members"=>
  [{"id"=>289,
    "group_id"=>1671,
    "created_by"=>nil,
    "updated_by"=>nil,
    "user"=>
     {"id"=>13496,
      "email"=>"generic_user@evanta.com",
      "alt_email"=>nil,
      "first_name"=>"Generic",
      "last_name"=>"User",
      "title"=>"CEO of QA",
      "organization_name"=>"Evanta",
      "bio"=>nil,
      "photo"=>
       "https://assets.evanta.com/shared/resources/Users/large/anonymous.jpg",
      "user_role_id"=>13500,
      "user_connection_id"=>nil}},
   {"id"=>290,
    "group_id"=>1671,
    "created_by"=>nil,
    "updated_by"=>nil,
    "user"=>
     {"id"=>13499,
      "email"=>"nickolas_keebler@kuvalis.biz",
      "alt_email"=>"brant@gmail.com",
      "first_name"=>"Forrest",
      "last_name"=>"Metz",
      "title"=>"Random User",
      "organization_name"=>"Kuhic and Sons",
      "bio"=>
       "Deleniti a quia incidunt amet voluptate natus cupiditate ex occaecati eos.",
      "photo"=>
       "https://assets.evanta.com/shared/resources/Users/large/anonymous.jpg",
      "user_role_id"=>13501,
      "user_connection_id"=>nil}}]}
```

This requests provides a <strong>HTML 200</strong> on success.