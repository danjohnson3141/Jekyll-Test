This is how the user will create a new group. On success of this route, a group_member record will be created for the active user and the new group.

=
#### Authentication

The user needs to be logged in and have valid credentials to use this route.

=
#### Parameters

:name - Varchar, passed in through the post data. Is derived from the 'name' field of the 'groups' table. This will be the name of the group

:description - Text, passed in through the post data. Is derived from the 'description' field of the 'groups' table. This will be the 

:group_type_id - Integer, passed in through the post data. Is derived from the 'id' field on 'group_types' table.

=
####JSON request example:
```
http://0.0.0.0:3000/groups
```

=
####JSON response example:

```
{"json_example"=>
  [{"id"=>123,
    "field1"=>"Text",
    "field2"=>nil
  }]
}
```

This requests provides a <strong>HTML 201</strong> on success.