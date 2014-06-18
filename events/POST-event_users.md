<!-- --- title: POST /event_users -->

This allows the user to create an event_user record. This route is still under development and will most likely be changing.

=
####Authentication:

The user needs to be logged in and have valid credentials to use this route.

=
####Parameters:

None; defaults only.

=
####Response:

This requests provides a <strong>HTML 201</strong> on success.

=
####API request example:
```html
http://example.com/event_users
```

=
####Post data example:
```
{ event_user: { event_id: 23, event_registration_status_id: @reg_stat.id } }
```
 
=
###Post data detail:

[[include:/post_data/post_event_user]]

=
####JSON response example:

[[include:/json/JSON_POST_event_users]]

=
####Response Data Detail:

[[include:/serializers/event_user]]