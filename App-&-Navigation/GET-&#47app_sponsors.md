<!-- --- title: GET /app_sponsors-->

This route is used to return a list of all of the application sponsors (these are different than event sponsors). 

=
#### Authentication
The user needs to be logged in and have valid credentials to use this route.

=
#### Parameters
none; only default response

=
####JSON request example:
```
http://0.0.0.0:3000/app_sponsors
```
=
####JSON response example:

```json
{"app_sponsors"=>
  [{"id"=>105,
    "name"=>"Harvey-Bruen",
    "description"=>
     "Delectus labore quia cum quaerat sed ratione qui et sit nam.",
    "logo"=>nil,
    "url"=>nil,
    "sponsor_type"=>
     {"id"=>144, "name"=>"A type of Sponsor", "description"=>"A Sponsor Type"},
    "users"=>[]},
   {"id"=>106,
    "name"=>"Zboncak Inc",
    "description"=>
     "Itaque officia quibusdam necessitatibus laboriosam consequatur officiis qui aspernatur unde.",
    "logo"=>nil,
    "url"=>nil,
    "sponsor_type"=>
     {"id"=>145, "name"=>"A type of Sponsor", "description"=>"A Sponsor Type"},
    "users"=>[]}]}
```

This request should provide a <strong>200 HTTP</strong> response when successful.