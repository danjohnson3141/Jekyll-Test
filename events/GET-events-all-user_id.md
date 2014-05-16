<!-- --- title: GET /events/all -->

Returns **all** the events for the active user for which they have _either_ an event_follower or event_user record. 

The events that are visible to the user are filtered by whether or not that event is associated with a group that the user is a member of. Being an event_user for an event trumps all group_member requirements.

=
####Authentication:

The user needs to be logged in and have valid credentials to use this route.

=
####Parameters:

None; default only

=
####API request example:
```json
http://stage-api-access.evant.com/events/all
```

=
####JSON response example:

```json
{"events"=>
  [{"id"=>13848,
    "name"=>"Rustic Granite Shoes 2",
    "event_begin_date"=>"2014-02-24",
    "event_end_date"=>"2014-02-26",
    "venue_name"=>"Bechtelar LLC",
    "address"=>"2155 Kennedy Mews",
    "state"=>"VI",
    "postal_code"=>"96743-7747",
    "event_follower_id"=>3122,
    "registraion_status"=>nil,
    "is_event_today"=>false,
    "can_follow_event"=>false,
    "country"=>{"id"=>3026, "name"=>"Korea", "abbreviation"=>"e4g"},
    "timezone"=>{"id"=>1112, "name"=>"Pacific", "offset"=>2},
    "group"=>
     {"id"=>16338, "name"=>"Open Group 3", "group_type_name"=>"Factory:Open"},
    "attendees"=>[]},
   {"id"=>13847,
    "name"=>"Sleek Cotton Hat 1",
    "event_begin_date"=>"2014-02-24",
    "event_end_date"=>"2014-02-26",
    "venue_name"=>"Fritsch Group",
    "address"=>"1441 Tracey Viaduct",
    "state"=>"CA",
    "postal_code"=>"45659",
    "event_follower_id"=>nil,
    "registraion_status"=>"attended",
    "is_event_today"=>false,
    "can_follow_event"=>false,
    "country"=>{"id"=>3025, "name"=>"Haiti", "abbreviation"=>"ne1"},
    "timezone"=>{"id"=>1111, "name"=>"Pacific", "offset"=>2},
    "group"=>
     {"id"=>16337, "name"=>"Open Group 2", "group_type_name"=>"Factory:Open"},
    "attendees"=>[]}]}
```

This requests provides a <strong>HTML 200</strong> on success.