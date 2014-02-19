Updates the group

=
#### Authentication

The user needs to be logged in and have valid credentials to use this route.

=
#### Parameters

:name - Varchar, passed in through the post data. Is derived from the 'name' field of the 'groups' table.

:description - Text, passed in through the post data. Is derived from the 'description' field of the 'groups' table.

=
####JSON request example:
```
http://0.0.0.0:3000/ROUTE_NAME
```

=
####JSON response example:

```
NO JSON RESPONSE
```

This requests provides a <strong>HTML 200</strong> on success.