<!-- --- title: POST /groups -->

This is how the user will create a new group. On success of this route, a group_member record will be created for the active user and the new group.

=
####Authentication:

The user needs to be logged in and have valid credentials to use this route.

=
####Parameters:

None; default only

=
####Response:

This requests provides a <strong>HTML 201</strong> on success.

=
####API request example:
```json
http://stage-api-access.evant.com/groups
```

=
####Post data example:
```
{ group: 
	{ name: "Awesome Saunce", 
	  group_type_id: 1, 
	  description: "Put it on your fries" } }
```

=
###Post data detail:

[[include:/post_data/post_groups]]

=
####JSON response example:

[[include:/json/JSON_POST_groups]]

=
####Response Data Detail:

[[include:/serializers/group]]