<!-- --- title: PUT /group_requests/:id -->

This is the method by which a group owner is able to approve the request of a different owner who requested to join that group.

=
#### Authentication

The user needs to be logged in and have valid credentials to use this route.

=
#### Parameters

(group_requests) :id - Integer, passed in the URL. Is derived from the 'id' field on the 'group_requests' table.

=
####JSON request example:
```json
http://0.0.0.0:3000/group_requests/234
```

=
####Post Data
```
NO POST DATA?
```

=
####JSON response example:

```json
NO JSON RESPONSE
```

This requests provides a <strong>HTML 204</strong> on success.