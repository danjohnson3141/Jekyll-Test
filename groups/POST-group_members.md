<!-- --- title: POST /group_members -->

This creates a new group membership record. The user associated with this record will always be the active user.

=
####Authentication

The user needs to be logged in and have valid credentials to use this route. 

=
####Parameters

None; default only.

=
####Response:

This requests provides a <strong>HTML 201</strong> on success.

=
####API request example:
```html
http://stage-api-access.evant.com/group_members
```

=
####Post data example:
```
{ group_member: 
  { group_id: 296 } 
```

=
###Post data detail:

[[include:/post_data/post_group_members]]

=
####JSON response example:

[[include:/json/JSON_POST_group_members]]

=
####Response data detail:

[[include:/serializers/group_member]]