Returns a list of all the events followed by one user.

=
#### Authentication

The user needs to be logged in and have valid credentials to use this route.

=
#### Parameters

:user_id - Integer, passed in through the URL. Is derived from the 'user_id' field on the 'event_followers' table.

=
####JSON request example:
```
http://0.0.0.0:3000/event_followers/events/35005
```

=
####JSON response example:

```
{"event_followers"=>
  [{"id"=>1032,
    "user_id"=>35005,
    "created_by"=>nil,
    "updated_by"=>nil,
    "event"=>
     {"id"=>4573,
      "name"=>"rspec test event 1",
      "event_begin_date"=>nil,
      "event_end_date"=>nil,
      "venue_name"=>nil,
      "address"=>nil,
      "state"=>nil,
      "postal_code"=>nil,
      "event_follower_id"=>1032,
      "registraion_status"=>nil,
      "is_event_today"=>nil,
      "can_follow_event"=>false,
      "country"=>nil,
      "timezone"=>nil,
      "group"=>
       {"id"=>5672, "name"=>"TestGroup", "group_type_name"=>"Factory:Open"},
      "attendees"=>[]}},
   {"id"=>1033,
    "user_id"=>35005,
    "created_by"=>nil,
    "updated_by"=>nil,
    "event"=>
     {"id"=>4574,
      "name"=>"rspec test event 2",
      "event_begin_date"=>nil,
      "event_end_date"=>nil,
      "venue_name"=>nil,
      "address"=>nil,
      "state"=>nil,
      "postal_code"=>nil,
      "event_follower_id"=>1033,
      "registraion_status"=>nil,
      "is_event_today"=>nil,
      "can_follow_event"=>false,
      "country"=>nil,
      "timezone"=>nil,
      "group"=>
       {"id"=>5672, "name"=>"TestGroup", "group_type_name"=>"Factory:Open"},
      "attendees"=>[]}}]}
```

This requests provides a <strong>HTML 200</strong> on success.