| name                      | description                                                         | type                            |
|---------------------------|---------------------------------------------------------------------|---------------------------------|
| id                        | The ID of this record                                               | integer                         |
| event_registration_status | Info on this users reg status                                       | object; EventRegistrationStatus |
| user                      | Info on the user                                                    | object; UserNano                |
| event                     | Info on the event                                                   | object; EventTiny               |
| sponsor                   | Info on the sponsor                                                 | object; SponsorTiny             |
| event_notes               | Any event notes that the active user may have created for this user | array; EventNoteTiny            |