<!-- --- title: PUT /groups/:id -->

Updates the group. Only the group owner is allowed to update the group, and the only editable options are the group's name and the description of the group.

=
####Authentication:

The user needs to be logged in and have valid credentials to use this route.

=
####Parameters:

:name - Varchar, passed in through the post data. Is derived from the 'name' field of the 'groups' table.

:description - Text, passed in through the post data. Is derived from the 'description' field of the 'groups' table.

=
####Response:

This requests provides a <strong>HTML 204</strong> on success.

=
####API request example:
```json
http://stage-api-access.evant.com/groups/234
```

=
####Post Data Example:
```
{ group: 
  { name: "Groups are Awesome", 
    description: "New Description" } 
 }
```

=
###Post data detail:

[[include:/post_data/patch_groups_id]]

=
####JSON response example:

[[include:/json/JSON_NO_RESPONSE]]