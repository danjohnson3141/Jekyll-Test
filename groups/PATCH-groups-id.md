<!-- --- title: PATCH /groups/:id -->

Updates the group. Only the group owner is allowed to update the group, and the only editable options are the group's name and the description of the group.

=
####Authentication:

The user needs to be logged in and have valid credentials to use this route.

=
####Parameters:

:id = The ID of the group to be edited.

=
####Response:

This requests provides a <strong>HTML 204</strong> on success.

=
####API request example:
```html
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