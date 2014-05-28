<!-- --- title: PUT /event_notes/:id -->

This allows the active user to edit **one** event_notes record. The active user is only able to update records for which they are the creator.

=
####Authentication:

The user needs to be logged in and have valid credentials to use this route.

=
####Parameters:

:id - Integer, passed in through the URL. Is derived from the 'id' field of the 'event_notes' table.

=
####Response:

This requests provides a <strong>HTML 204</strong> on success.

=
####API request example:
```html
http://stage-api-access.evant.com/event_notes/234
```

=
####Post data example:
```
{ event_note: { body: 'This is the updated body of the event note.' } }
```

=
###Post data detail:

[[include:/post_data/patch_event_notes_id]]

=
####JSON response example:

[[include:/json/JSON_NO_RESPONSE]]
