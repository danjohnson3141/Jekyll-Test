<!-- --- title: POST /event_users -->

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
http://0.0.0.0:3000/event_users
```

=
####Post Data
```
{ event_user: 
  { user_id: 4890, 
    event_id: 42 } 
}
```

=
####JSON response example:

```json
{"event_user"=>
  {"id"=>134,
   "created_by"=>nil,
   "updated_by"=>nil,
   "event_registration_status"=>nil,
   "user"=>
    {"id"=>4890,
     "email"=>"generic_user@evanta.com",
     "alt_email"=>"alt_gen_use@evanta.com",
     "first_name"=>"Generic",
     "last_name"=>"User",
     "title"=>"CEO of QA",
     "organization_name"=>"Evanta",
     "bio"=>"This is the biography of the default Generic User",
     "photo"=>
      "https://assets.evanta.com/shared/resources/Users/large/anonymous2.jpg",
     "user_role_id"=>4864,
     "user_connection_id"=>nil},
   "event"=>
    {"id"=>442,
     "name"=>"rspec test event",
     "begin_date"=>"2014-02-24",
     "end_date"=>"2014-02-26",
     "venue_name"=>nil,
     "address"=>nil,
     "state"=>nil,
     "postal_code"=>nil,
     "event_follower_id"=>nil,
     "registraion_status"=>nil,
     "is_event_today"=>false,
     "can_follow_event"=>true,
     "country"=>nil,
     "timezone"=>nil,
     "group"=>
      {"id"=>1054, "name"=>"rspec test group", "group_type_name"=>"Open"},
     "attendees"=>[]},
   "event_sponsor"=>nil}}
```

This requests provides a <strong>HTML 201</strong> on success.