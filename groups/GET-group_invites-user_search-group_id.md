<!-- --- title: GET /group_invites/user_search/:group_id -->

This is a route for searching for other users that the active user can invite to their group. Functionality for this route is still in development. Generally speaking, this route should work by passing in a text string and a group_id and returning a list of potential members.

=
####Authentication:

The user needs to be logged in and have valid credentials to use this route.

=
####Parameters:

:group_id - Integer, passed in through the URL. Is derived from the 'id' field on the 'groups' table.
?query= - Text, passed in through the URL. Text that will be searched for.

=
####Response:

This requests provides a <strong>HTML 200</strong> on success.

=
####API request example:
```html
http://example.com/group_invites/user_search/4?query=bry
```

=
####JSON response example:

returns an array of UserNano

[[include:/json/JSON_GET_group_invites_user_search_group_id]]

=
####Response Data Detail:

[[include:/serializers/user_nano]]