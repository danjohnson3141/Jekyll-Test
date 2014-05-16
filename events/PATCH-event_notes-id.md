<!-- --- title: PATCH /event_notes/:id -->

This allows the active user to update **one** event_notes record.

=
####Authentication:

The user needs to be logged in and have valid credentials to use this route.

=
####Parameters:

(event_notes) :id - Integer, passed in through the URL. Is derived from the 'id' field of the 'event_notes' table.

:body - Text, passed in through the post data. This is the plain text of the submission.

=
####API request example:
```json
http://stage-api-access.evant.com/event_notes/234
```

=
####Post data example:
```
{ event_note: { body: 'This is the updated body of the event note.' } }
```

=
####JSON response example:

[[include:/json/JSON_NO_RESPONSE]]

This requests provides a <strong>HTML 204</strong> on success.