<!-- --- title: POST /event_notes -->

Allows the active user to create a note. Each note is able to reference **one** and **only** one of the following: event_user, sponsor_id, event_speaker_id, or event_session_id. If the user attempts to pass in more than one of these, the request will fail.

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
http://stage-api-access.evant.com/event_notes
```

####Post Data::
```
{ event_note: { body: 'This text is the body of the note.', event_session_id: 21 }
```

=
###Post data detail:

[[include:/post_data/post_event_notes]]


=
####JSON response example:

[[include:/json/JSON_POST_event_notes]]

=
####Response Data Detail:

[[include:/serializers/event_note]]