<!-- --- title: GET /navigation/right/:event_id -->

This returns the elements for the right navigation bar. It has something to do 

=
#### Authentication

Declare what authentications are required
Good sample text: The user needs to be logged in and have valid credentials to use this route.

=
#### Parameters

:event_id - Integer, passed in through the URL. Derived from the 'id' field of the 'events' table.

=
####JSON request example:
```
http://0.0.0.0:3000/navigation/right/234
```

=
####JSON response example:

```
{"navigation_right"=>
  {"show_attendees"=>false,
   "show_sessions"=>false,
   "show_my_schedule"=>false,
   "show_sponsors"=>false,
   "show_speakers"=>false,
   "show_qr_scannable"=>false,
   "show_qr_scanner"=>false,
   "show_event_notes"=>false,
   "show_bookmarks"=>false,
   "show_leaderboard"=>false,
   "show_leaderboard_rules"=>false,
   "show_event_evaluations"=>false}}
```

This requests provides a <strong>HTML 200</strong> on success.