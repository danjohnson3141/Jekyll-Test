| name         | description                             | type              |
|--------------|-----------------------------------------|-------------------|
| id           | The ID of this record                   | integer           |
| name         | The name of this event_council          | string            |
| display_rank | Allows for arbitrary sorting of results | integer           |
| client_id    | A reference key to an external record   | string            |
| event        | Info on the event                       | object; EventTiny |