<!-- --- title: GET /events -->

Returns **all** events that are visible to the user.

The events that are visible to the user are filtered by whether or not that event is associated with a group that the user is a member of. Being an event_user for an event trumps all group_member requirements.

=
#### Authentication

The user needs to be logged in and have valid credentials to use this route.

=
#### Parameters

none; default only.

=
####API request example:
```json
http://stage-api-access.evant.com/events
```

=
####JSON response example:

```json
{"events"=>
  [{"id"=>16315,
    "name"=>"Awesome Concrete Shoes 12",
    "event_begin_date"=>"2014-03-07",
    "event_end_date"=>"2014-03-08",
    "venue_name"=>"Macejkovic, Kunze and Gutmann",
    "address"=>"58994 Marks Circle",
    "state"=>"WI",
    "postal_code"=>"53715",
    "event_follower_id"=>nil,
    "registraion_status"=>nil,
    "is_event_today"=>false,
    "can_follow_event"=>false,
    "country"=>{"id"=>4136, "name"=>"Nauru", "abbreviation"=>"86d"},
    "timezone"=>{"id"=>2222, "name"=>"Pacific", "offset"=>2},
    "group"=>
     {"id"=>18431, "name"=>"Open Group 13", "group_type_name"=>"Factory:Open"},
    "attendees"=>[]},
   {"id"=>16314,
    "name"=>"Rustic Plastic Shirt 11",
    "event_begin_date"=>"2014-03-07",
    "event_end_date"=>"2014-03-08",
    "venue_name"=>"Harvey Inc",
    "address"=>"704 Rau Views",
    "state"=>"UT",
    "postal_code"=>"38416",
    "event_follower_id"=>nil,
    "registraion_status"=>nil,
    "is_event_today"=>false,
    "can_follow_event"=>false,
    "country"=>{"id"=>4135, "name"=>"Malaysia", "abbreviation"=>"l85"},
    "timezone"=>{"id"=>2221, "name"=>"Pacific", "offset"=>2},
    "group"=>
     {"id"=>18430, "name"=>"Open Group 12", "group_type_name"=>"Factory:Open"},
    "attendees"=>[]}]}
```

This requests provides a <strong>HTML 200</strong> on success.