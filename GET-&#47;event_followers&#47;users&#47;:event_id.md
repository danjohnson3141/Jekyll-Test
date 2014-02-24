PLAIN ENGLISH DESCRIPTION OF THE ROUTE

=
#### Authentication

Declare what authentications are required

Good sample text: The user needs to be logged in and have valid credentials to use this route.

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

This requests provides a <strong>HTML RESPONSE NUMBER</strong> on success.