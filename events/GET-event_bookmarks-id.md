<!-- --- title: GET /event_bookmarks/:id -->

Returns **one** event bookmark based on the id passed in.

=
####Authentication:

The user needs to be logged in and have valid credentials to use this route.

=
####Parameters:

(event_bookmarks) :id - Integer, passed in the URL. Is derived from the 'id' field on the the 'event_bookmarks' table.

=
####API request example:
```json
http://stage-api-access.evant.com/event_bookmarks/81
```

=
####JSON response example:

```json
{"event_bookmark"=>
  {"id"=>81,
   "event"=>{"id"=>159, "name"=>"Small Wooden Shoes 137"},
   "event_user"=>nil,
   "event_speaker"=>
    {"id"=>33,
     "user_id"=>1155,
     "first_name"=>"Alisha",
     "last_name"=>"Kessler",
     "title"=>"Rustic Cotton Gloves",
     "organization_name"=>"Schuppe-O'Reilly",
     "bio"=>
      "Et est qui corrupti voluptas. Ea et nesciunt accusamus. Quas maiores totam voluptas ea nihil amet saepe. Quas dolores ut.\n\nLibero harum sed. Doloremque totam voluptas. Praesentium quidem fugit.",
     "speaker_type"=>"Gorgeous Concrete Hat",
     "photo"=>
      "https://assets.evanta.com/shared/resources/Users/large/anonymous2.jpg",
     "event_session_id"=>127},
   "event_session"=>nil,
   "sponsor"=>nil}}
```

This requests provides a <strong>HTML 200</strong> on success.