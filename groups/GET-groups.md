<!-- --- title: GET /groups -->

Returns a list of all groups that are visible to the active user. Secret groups that the user is not a member of will not be returned. 

=
#### Authentication

The user needs to be logged in and have valid credentials to use this route.

=
#### Parameters

none; default only

=
####JSON request example:
```json
http://stage-api-access.evant.com/groups
```

=
####JSON response example:

[[include:/json/GET groups json.md]]

```json
```

This requests provides a <strong>HTML 200</strong> on success.