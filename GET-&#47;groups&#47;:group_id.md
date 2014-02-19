Returns details on *one* group.

=
#### Authentication

The user needs to be logged in and have valid credentials to use this route.

=
#### Parameters

:group_id - Integer, passed in through the URL. Is derived from the 'id' field on the 'groups' table.

=
####JSON request example:
```
http://0.0.0.0:3000/ROUTE_NAME
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

This requests provides a <strong>HTML RESPONSE NUMBER</strong> on success.