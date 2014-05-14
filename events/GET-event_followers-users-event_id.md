<!-- --- title: GET /event_followers/users/:event_id -->

Returns all of the followers for one event.

=
####Authentication:

The user needs to be logged in and have valid credentials to use this route.

=
####Parameters:

:event_id - Integer, passed in through the URL. Is derived from the 'event_id' field on the 'event_followers'

=
####API request example:
```json
http://stage-api-access.evant.com/event_followers/users/4739
```

=
####JSON response example:

```json
{"event_followers"=>
  [{"id"=>1074,
    "event_id"=>4739,
    "created_by"=>nil,
    "updated_by"=>nil,
    "user"=>
     {"id"=>36778,
      "email"=>"generic_user@evanta.com",
      "alt_email"=>nil,
      "first_name"=>"Generic",
      "last_name"=>"User",
      "title"=>"CEO of QA",
      "organization_name"=>"Evanta",
      "bio"=>"This is the biography of the default Generic User",
      "photo"=>
       "https://assets.evanta.com/shared/resources/Users/large/anonymous2.jpg",
      "user_role_id"=>36782,
      "user_connection_id"=>nil}},
   {"id"=>1075,
    "event_id"=>4739,
    "created_by"=>nil,
    "updated_by"=>nil,
    "user"=>
     {"id"=>36781,
      "email"=>"brisa@fadel.org",
      "alt_email"=>"marlee_borer@gmail.com",
      "first_name"=>"Darion",
      "last_name"=>"Lang",
      "title"=>"Random User",
      "organization_name"=>"McClure Group",
      "bio"=>
       "Itaque perspiciatis adipisci magnam magni aut reprehenderit ex deleniti aut nostrum.",
      "photo"=>
       "https://assets.evanta.com/shared/resources/Users/large/anonymous2.jpg",
      "user_role_id"=>36783,
      "user_connection_id"=>nil}}]}
```

This requests provides a <strong>HTML 200</strong> on success.