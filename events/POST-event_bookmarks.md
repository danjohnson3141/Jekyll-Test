<!-- --- title: POST /event_bookmarks -->

Allows the active user to create a bookmark. Each bookmark is able to reference **one** and **only** one of the following: event_user, sponsor_id, event_speaker_id, or event_session_id. If the user attempts to pass in more than one of these, the request will fail.

=
####Authentication:

The user needs to be logged in and have valid credentials to use this route.

=
####Parameters:

none, default only.

=
####Response:

This requests provides a <strong>HTML 201</strong> on success.

=
####API request example:
```json
http://stage-api-access.evant.com/event_bookmarks
```

=
####Post data example::
```
{ event_bookmark: 
  { event_session_id: 9 } }
```

=
###Post data detail:

[[include:/post_data/post_event_bookmark]]


=
####JSON response example:

[[include:/json/JSON_POST_event_bookmarks]]

=
####Response Data Detail:

[[include:/serializers/event_bookmark_short]]