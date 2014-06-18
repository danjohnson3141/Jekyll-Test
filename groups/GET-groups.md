<!-- --- title: GET /groups -->

Returns a list of all groups that are visible to the active user. Secret groups that the user is not a member of will not be returned. This route returns a lot more data than seems neccessary, but that's because the front end resuses a lot of this data through the UX.

=
####Authentication

The user needs to be logged in and have valid credentials to use this route.

=
####Parameters

None; default only..

=
####Response:

This requests provides a <strong>HTML 200</strong> on success.

=
####API request example:
```html
http://example.com/groups
```

=
####JSON response example:

Returns an array of group objects

[[include:/json/JSON_GET_groups]]

=
####Response Data Detail:

[[include:/serializers/group]]