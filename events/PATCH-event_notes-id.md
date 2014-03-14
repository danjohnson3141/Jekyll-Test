<!-- --- title: PATCH /event_notes/:id -->

This allows the active user to update **one** event_notes record.

=
#### Authentication

The user needs to be logged in and have valid credentials to use this route.

=
#### Parameters

(event_notes) :id - Integer, passed in through the URL. Is derived from the 'id' field of the 'event_notes' table.

:body - Text, passed in through the post data. This is the plain text of the submission.

=
####JSON request example:
```json
http://0.0.0.0:3000/event_notes/234
```

=
####Post Data
```
{ event_note: { body: 'This is the updated body of the event note.' } }
```

=
####JSON response example:

```json
NO JSON RESPONSE
```

This requests provides a <strong>HTML 204</strong> on success.