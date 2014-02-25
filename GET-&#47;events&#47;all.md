Returns all the events.

=
#### Authentication

The user needs to be logged in and have valid credentials to use this route.

=
#### Parameters

LIST OF ALL PARAMETERS AND WHAT THEY ARE

=
####JSON request example:
```
http://0.0.0.0:3000/ROUTE_NAME
```

=
####JSON response example:

```
{"events"=>
  [{"id"=>15757,
    "name"=>"Test Event 0",
    "event_begin_date"=>"2014-03-07",
    "event_end_date"=>"2014-03-08",
    "venue_name"=>"Emmerich-Watsica",
    "address"=>"935 Gisselle Forge",
    "state"=>"MS",
    "postal_code"=>"95583-1039",
    "event_follower_id"=>nil,
    "registraion_status"=>nil,
    "is_event_today"=>false,
    "can_follow_event"=>false,
    "country"=>{"id"=>3857, "name"=>"Nigeria", "abbreviation"=>"qj0"},
    "timezone"=>{"id"=>1943, "name"=>"Pacific", "offset"=>2},
    "group"=>
     {"id"=>17744, "name"=>"Open Group 1", "group_type_name"=>"Factory:Open"},
    "attendees"=>[]},
   {"id"=>15758,
    "name"=>"Test Event 1",
    "event_begin_date"=>"2014-03-07",
    "event_end_date"=>"2014-03-08",
    "venue_name"=>"Pacocha, Jacobi and Franecki",
    "address"=>"852 Lynch Pass",
    "state"=>"NH",
    "postal_code"=>"97699",
    "event_follower_id"=>nil,
    "registraion_status"=>nil,
    "is_event_today"=>false,
    "can_follow_event"=>false,
    "country"=>{"id"=>3858, "name"=>"Switzerland", "abbreviation"=>"3vp"},
    "timezone"=>{"id"=>1944, "name"=>"Pacific", "offset"=>2},
    "group"=>
     {"id"=>17744, "name"=>"Open Group 1", "group_type_name"=>"Factory:Open"},
    "attendees"=>[]}]}
```

This requests provides a <strong>HTML 200</strong> on success.