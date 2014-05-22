<!-- --- title: POST /event_followers -->

This creates the event_followers records. The user should only be able to post records for their own account.

=
####Authentication:

The user needs to be logged in and have valid credentials to use this route.

=
####Parameters:

None; default only.

=
####Response:

This requests provides a <strong>HTML 201</strong> on success.

=
####API request example:
```json
http://stage-api-access.evant.com/event_followers
```

=
####Post data example::
```
{ event_follower: 
  { event_id: 18374 } }
```
 
=
###Post data detail:

[[include:/post_data/post_event_followers]]

=
####JSON response example:

[[include:/json/JSON_POST_event_followers]]

=
####Response Data Detail:

[[include:/serializers/event_follower]]