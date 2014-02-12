This route is used to populate the various text form elements on each page. The database groups these into 'dictionaries' for each page of the application and returns all the labels for that page rather than having the API ask for each label individually. 

Some requests do not require the user to be authenticated, this is determined by the 'auth_required' field of the app_label_pages table in the database (0 = auth not required, 1 = auth required).

=
#### Parameters

=
####JSON request example:
```
http://0.0.0.0:3000/app_sponsors
```
=
####JSON response example:

```
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

This request should provide a <strong>200 HTTP</strong> response when successful and a 404 when it fails.