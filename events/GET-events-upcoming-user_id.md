<!-- --- title: GET /events/upcoming -->

Returns a list of **all** upcoming events that are visible to the active user.

The events that are visible to the user are filtered by whether or not that event is associated with a group that the user is a member of. Being an event_user for an event trumps all group_member requirements.

=
####Authentication:

The user needs to be logged in and have valid credentials to use this route.

=
####Parameters:

none; default only

=
####API request example:
```json
http://stage-api-access.evant.com/events/upcoming
```

=
####JSON response example:

```json
{"events"=>
  [{"id"=>18238,
    "name"=>"Ergonomic Steel Chair 18",
    "event_begin_date"=>"2014-03-07",
    "event_end_date"=>"2014-03-08",
    "venue_name"=>"Wuckert LLC",
    "address"=>"52923 Berniece Creek",
    "state"=>"OH",
    "postal_code"=>"83864",
    "event_follower_id"=>4245,
    "registraion_status"=>nil,
    "is_event_today"=>false,
    "can_follow_event"=>false,
    "country"=>{"id"=>5004, "name"=>"French Guiana", "abbreviation"=>"2ij"},
    "timezone"=>{"id"=>3090, "name"=>"Pacific", "offset"=>2},
    "group"=>
     {"id"=>19776, "name"=>"Open Group 19", "group_type_name"=>"Factory:Open"},
    "attendees"=>[]},
   {"id"=>18237,
    "name"=>"Small Plastic Gloves 17",
    "event_begin_date"=>"2014-03-07",
    "event_end_date"=>"2014-03-08",
    "venue_name"=>"Langworth-Greenfelder",
    "address"=>"8270 Farrell Parks",
    "state"=>"MH",
    "postal_code"=>"92378-2141",
    "event_follower_id"=>nil,
    "registraion_status"=>"registered",
    "is_event_today"=>false,
    "can_follow_event"=>false,
    "country"=>{"id"=>5003, "name"=>"Malta", "abbreviation"=>"79f"},
    "timezone"=>{"id"=>3089, "name"=>"Pacific", "offset"=>2},
    "group"=>
     {"id"=>19775, "name"=>"Open Group 18", "group_type_name"=>"Factory:Open"},
    "attendees"=>[]}]}```

This requests provides a <strong>HTML 200</strong> on success.