<!-- --- title: GET /event_users/users/:event_id -->

This returns all the event users for one event.

=
#### Authentication

The user needs to be logged in and have valid credentials to use this route.

=
#### Parameters

:event_id - Integer, passed in through the URL. Is derived from the 'event_id' field on the 'event_users' table.

=
####JSON request example:
```
http://0.0.0.0:3000/event_users/users/10579
```

=
####JSON response example:

```
{"event_followers"=>
  [{"id"=>2344,
    "event_id"=>10579,
    "created_by"=>nil,
    "updated_by"=>nil,
    "user"=>
     {"id"=>83483,
      "email"=>"generic_user@evanta.com",
      "alt_email"=>"alt_gen_use@evanta.com",
      "first_name"=>"Generic",
      "last_name"=>"User",
      "title"=>"CEO of QA",
      "organization_name"=>"Evanta",
      "bio"=>"This is the biography of the default Generic User",
      "photo"=>
       "https://assets.evanta.com/shared/resources/Users/large/anonymous2.jpg",
      "user_role_id"=>83487,
      "user_connection_id"=>nil}},
   {"id"=>2345,
    "event_id"=>10579,
    "created_by"=>nil,
    "updated_by"=>nil,
    "user"=>
     {"id"=>83486,
      "email"=>"garrison.hayes@wizakunze.name",
      "alt_email"=>"herta@hotmail.com",
      "first_name"=>"Ines",
      "last_name"=>"Ledner",
      "title"=>"Random User",
      "organization_name"=>"Bergnaum LLC",
      "bio"=>
       "Vitae illum non culpa qui dolores nulla et reprehenderit eos qui id sed adipisci praesentium.",
      "photo"=>
       "https://assets.evanta.com/shared/resources/Users/large/anonymous2.jpg",
      "user_role_id"=>83488,
      "user_connection_id"=>1020}}]}
```

This requests provides a <strong>HTML 200</strong> on success.