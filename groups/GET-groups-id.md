<!-- --- title: GET /groups/:id -->

Returns details on **one** group.

=
####Authentication:

The user needs to be logged in and have valid credentials to use this route.

=
####Parameters:

:group_id - Integer, passed in through the URL. Is derived from the 'id' field on the 'groups' table.

=
####Response:
This requests provides a <strong>HTML 200</strong> on success.

=
####API request example:
```html
http://example.com/groups/2315
```

=
####JSON response example:

[[include:/json/JSON_GET_groups_id]]

=
####Response Data Detail:

[[include:/serializers/group]]