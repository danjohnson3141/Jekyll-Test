<!-- --- title: GET /events/:event_id -->

Returns the details for one event.

=
#### Authentication

The user needs to be logged in and have valid credentials to use this route.

=
#### Parameters

:event_id - Integer, passed in through the URL. Is derived from the 'id' field of the 'events' table.

=
####JSON request example:
```json
http://0.0.0.0:3000/events/11787
```

=
####JSON response example:

```json
{"event"=>
  {"id"=>11787,
   "name"=>"Small Cotton Pants 42",
   "event_begin_date"=>"2014-02-25",
   "event_end_date"=>"2014-02-25",
   "venue_name"=>"Schmeler, Parisian and Beahan",
   "address"=>"41038 Luettgen Springs",
   "state"=>"SD",
   "postal_code"=>"15296-5016",
   "event_follower_id"=>2613,
   "registraion_status"=>"registered",
   "is_event_today"=>true,
   "can_follow_event"=>false,
   "country"=>{"id"=>2173, "name"=>"Botswana", "abbreviation"=>"whv"},
   "timezone"=>{"id"=>259, "name"=>"Pacific", "offset"=>2},
   "group"=>
    {"id"=>14130, "name"=>"Open Group 47", "group_type_name"=>"Factory:Open"},
   "attendees"=>[]}}
```

This requests provides a <strong>HTML 200</strong> on success.