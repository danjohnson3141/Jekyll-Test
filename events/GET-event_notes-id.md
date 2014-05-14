<!-- --- title: GET /event_notes/:id -->

Returns **one** event note based on the data passed in.

=
####Authentication:

The user needs to be logged in and have valid credentials to use this route.

=
####Parameters:

(event_notes) :id - Integer, passed in through the URL. Is derived from the 'id' field of the 'event_notes' table.

=
####API request example:
```json
http://stage-api-access.evant.com/event_notes/14
```

=
####JSON response example:

```json
{"event_note"=>
  {"id"=>14,
   "body"=>
    "Facilis omnis totam molestias quis animi exercitationem. Est non nam sint suscipit. Cum voluptatem in est recusandae deserunt ducimus aliquam.\n\nSit mollitia vel sequi. Velit totam temporibus quam. Deleniti consectetur animi explicabo est.",
   "event"=>{"id"=>35, "name"=>"Gorgeous Wooden Chair 35"},
   "event_user"=>
    {"id"=>31,
     "user"=>
      {"id"=>1689,
       "first_name"=>"Generic",
       "last_name"=>"User",
       "title"=>"CEO of QA",
       "organization_name"=>"Evanta",
       "photo"=>
        "https://assets.evanta.com/shared/resources/Users/large/anonymous2.jpg",
       "user_role_id"=>46254,
       "user_connection_id"=>nil}},
   "event_speaker"=>nil,
   "event_session"=>nil,
   "sponsor"=>nil}}
```

This requests provides a <strong>HTML 200</strong> on success.