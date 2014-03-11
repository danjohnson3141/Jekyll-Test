<!-- --- title: GET /events/past -->

Returns a list of all events whose date is before today.

=
#### Authentication

The user needs to be logged in and have valid credentials to use this route.

=
#### Parameters

none; default only

=
####JSON request example:
```json
http://0.0.0.0:3000/events/past
```

=
####JSON response example:

```json
{"events"=>
  [{"id"=>16960,
    "name"=>"Rustic Concrete Pants 2",
    "event_begin_date"=>"2014-02-24",
    "event_end_date"=>"2014-02-26",
    "venue_name"=>"Schowalter, Waelchi and Kertzmann",
    "address"=>"54323 Jacobs Track",
    "state"=>"DC",
    "postal_code"=>"78903-0349",
    "event_follower_id"=>nil,
    "registraion_status"=>nil,
    "is_event_today"=>false,
    "can_follow_event"=>false,
    "country"=>{"id"=>4418, "name"=>"Isle of Man", "abbreviation"=>"7d9"},
    "timezone"=>{"id"=>2504, "name"=>"Pacific", "offset"=>2},
    "group"=>
     {"id"=>19079, "name"=>"Open Group 3", "group_type_name"=>"Factory:Open"},
    "attendees"=>[]},
   {"id"=>16959,
    "name"=>"Rustic Rubber Hat 1",
    "event_begin_date"=>"2014-02-24",
    "event_end_date"=>"2014-02-26",
    "venue_name"=>"Kuvalis-Gleichner",
    "address"=>"99963 Rau Fall",
    "state"=>"WI",
    "postal_code"=>"23903",
    "event_follower_id"=>nil,
    "registraion_status"=>nil,
    "is_event_today"=>false,
    "can_follow_event"=>false,
    "country"=>{"id"=>4417, "name"=>"Spain", "abbreviation"=>"dxu"},
    "timezone"=>{"id"=>2503, "name"=>"Pacific", "offset"=>2},
    "group"=>
     {"id"=>19078, "name"=>"Open Group 2", "group_type_name"=>"Factory:Open"},
    "attendees"=>[]}]}
```

This requests provides a <strong>HTML 200</strong> on success.