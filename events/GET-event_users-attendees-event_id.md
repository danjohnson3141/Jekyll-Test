<!-- --- title: GET /event_users/attendees/:event_id -->

Returns all of the event users for one event.

=
#### Authentication

The user needs to be logged in and have valid credentials to use this route.

=
#### Parameters

:event_id - Integer, passed in through the URL. Is derived from the 'event_id' field on the 'event_users' table.

=
####JSON request example:
```json
http://0.0.0.0:3000/event_users/attendees/7704
```

=
####JSON response example:

```json
"event_users"=>
  [{"id"=>2589,
    "event_id"=>7704,
    "user"=>
     {"id"=>60321,
      "first_name"=>"Lloyd",
      "last_name"=>"Aardvark",
      "title"=>"Random User",
      "organization_name"=>"Boyer, Deckow and Barrows",
      "photo"=>
       "https://assets.evanta.com/shared/resources/Users/large/anonymous2.jpg",
      "user_role_id"=>60323},
    "event_registration_status"=>{"id"=>638, "key"=>"registered"}},
   {"id"=>2590,
    "event_id"=>7704,
    "user"=>
     {"id"=>60318,
      "first_name"=>"Haylee",
      "last_name"=>"Zebra",
      "title"=>"Random User",
      "organization_name"=>"Glover Group",
      "photo"=>
       "https://assets.evanta.com/shared/resources/Users/large/anonymous2.jpg",
      "user_role_id"=>60320},
    "event_registration_status"=>{"id"=>639, "key"=>"attended"}}]}
```

This requests provides a <strong>HTML 200</strong> on success.