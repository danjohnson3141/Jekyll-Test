<!-- --- title: GET /events/upcoming -->

Returns a list of all upcoming events.

=
#### Authentication

The user needs to be logged in and have valid credentials to use this route.

=
#### Parameters

none; defaults only

=
####JSON request example:
```
http://0.0.0.0:3000/events/upcoming
```

=
####JSON response example:

```
{"events"=>
  [{"id"=>18150,
    "name"=>"Awesome Concrete Chair 17",
    "event_begin_date"=>"2014-03-07",
    "event_end_date"=>"2014-03-08",
    "venue_name"=>"Gerlach, Hayes and Jerde",
    "address"=>"302 Heath Center",
    "state"=>"MD",
    "postal_code"=>"76914",
    "event_follower_id"=>nil,
    "registraion_status"=>nil,
    "is_event_today"=>false,
    "can_follow_event"=>false,
    "country"=>{"id"=>4946, "name"=>"Tuvalu", "abbreviation"=>"oi3"},
    "timezone"=>{"id"=>3032, "name"=>"Pacific", "offset"=>2},
    "group"=>
     {"id"=>19725, "name"=>"Open Group 16", "group_type_name"=>"Factory:Open"},
    "attendees"=>[]},
   {"id"=>18149,
    "name"=>"Sleek Rubber Chair 16",
    "event_begin_date"=>"2014-03-07",
    "event_end_date"=>"2014-03-08",
    "venue_name"=>"Simonis, Kohler and Kuphal",
    "address"=>"4665 Shanahan Glen",
    "state"=>"CT",
    "postal_code"=>"94453-2857",
    "event_follower_id"=>nil,
    "registraion_status"=>nil,
    "is_event_today"=>false,
    "can_follow_event"=>false,
    "country"=>{"id"=>4945, "name"=>"Uganda", "abbreviation"=>"7ku"},
    "timezone"=>{"id"=>3031, "name"=>"Pacific", "offset"=>2},
    "group"=>
     {"id"=>19724, "name"=>"Open Group 15", "group_type_name"=>"Factory:Open"},
    "attendees"=>[]}]}
```

This requests provides a <strong>HTML 200</strong> on success.