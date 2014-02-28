This creates the event_followers records. The user should only be able to post records for their own account.

=
#### Authentication

The user needs to be logged in and have valid credentials to use this route.

=
#### Parameters

LIST OF ALL PARAMETERS AND WHAT THEY ARE

=
####JSON request example:
```
http://0.0.0.0:3000/event_followers
```

=
####Post Data:
```
{ event_follower: 
  { user_id: 129457, 
    event_id: 18374 } 
 }
```
=
####JSON response example:

```
{"event_follower"=>
  {"id"=>4283,
   "created_by"=>nil,
   "updated_by"=>nil,
   "user"=>
    {"id"=>129457,
     "email"=>"generic_user@evanta.com",
     "alt_email"=>"alt_gen_use@evanta.com",
     "first_name"=>"Generic",
     "last_name"=>"User",
     "title"=>"CEO of QA",
     "organization_name"=>"Evanta",
     "bio"=>"This is the biography of the default Generic User",
     "photo"=>
      "https://assets.evanta.com/shared/resources/Users/large/anonymous2.jpg",
     "user_role_id"=>129461,
     "user_connection_id"=>nil},
   "event"=>
    {"id"=>18374,
     "name"=>"Sleek Granite Computer 1",
     "event_begin_date"=>"2014-03-07",
     "event_end_date"=>"2014-03-08",
     "venue_name"=>"Hills-Strosin",
     "address"=>"74058 Madisyn Pines",
     "state"=>"VA",
     "postal_code"=>"18034",
     "event_follower_id"=>4283,
     "registraion_status"=>nil,
     "is_event_today"=>false,
     "can_follow_event"=>false,
     "country"=>{"id"=>5110, "name"=>"Serbia", "abbreviation"=>"08j"},
     "timezone"=>{"id"=>3196, "name"=>"Pacific", "offset"=>2},
     "group"=>
      {"id"=>19839, "name"=>"Open Group 1", "group_type_name"=>"Factory:Open"},
     "attendees"=>[]}}}
```

This requests provides a <strong>HTML 201</strong> on success.