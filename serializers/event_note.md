| name          | description               | type                      |
|---------------|---------------------------|---------------------------|
| id            | The ID of this record     | integer                   |
| body          | Content of the note       | string                    |
| event         | Info on the event         | object; EventTiny         |
| event_user    | Info on the event_user    | object; EventUserTiny     |
| event_speaker | Info on the event_speaker | object; EventSpeakerShort |
| event_session | Info on the event_session | object; EventSessionShort |
| sponsor       | Info on the sponsor       | object; SponsorTiny       |