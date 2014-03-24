<!-- --- title: GET /events/past/:user_id -->

Returns **all** of the past events that are visible to the active user.

The events that are visible to the user are filtered by whether or not that event is associated with a group that the user is a member of. Being an event_user for an event trumps all group_member requirements.

=
#### Authentication

The user needs to be logged in and have valid credentials to use this route.

=
#### Parameters

:user_id - Integer, passed in through the URL. Is derived from the 'id' field on the 'users' table.

=
####JSON request example:
```json
http://0.0.0.0:3000/events/past/125861
```

=
####JSON response example:

```json
{"events"=>
  [{"id"=>17627,
    "name"=>"Intelligent Rubber Shirt 8",
    "event_begin_date"=>"2014-02-24",
    "event_end_date"=>"2014-02-26",
    "venue_name"=>"Bergstrom, Quigley and Frami",
    "address"=>"66001 Gloria Spur",
    "state"=>"RI",
    "postal_code"=>"39145-7656",
    "event_follower_id"=>nil,
    "registraion_status"=>"attended",
    "is_event_today"=>false,
    "can_follow_event"=>false,
    "country"=>{"id"=>4645, "name"=>"Kuwait", "abbreviation"=>"qd0"},
    "timezone"=>{"id"=>2731, "name"=>"Pacific", "offset"=>2},
    "group"=>
     {"id"=>19203, "name"=>"Open Group 7", "group_type_name"=>"Factory:Open"},
    "attendees"=>[]},
   {"id"=>17628,
    "name"=>"Intelligent Steel Gloves 9",
    "event_begin_date"=>"2014-02-24",
    "event_end_date"=>"2014-02-26",
    "venue_name"=>"Welch, Maggio and Walker",
    "address"=>"312 Luz Valleys",
    "state"=>"MO",
    "postal_code"=>"98719-1447",
    "event_follower_id"=>4074,
    "registraion_status"=>nil,
    "is_event_today"=>false,
    "can_follow_event"=>false,
    "country"=>
     {"id"=>4646, "name"=>"Russian Federation", "abbreviation"=>"amy"},
    "timezone"=>{"id"=>2732, "name"=>"Pacific", "offset"=>2},
    "group"=>
     {"id"=>19204, "name"=>"Open Group 8", "group_type_name"=>"Factory:Open"},
    "attendees"=>[]}]}
```

This requests provides a <strong>HTML 200</strong> on success.