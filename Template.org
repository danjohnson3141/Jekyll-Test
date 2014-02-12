PLAIN ENGLISH DESCRIPTION OF THE ROUTE

=
#### Authentication

Declare what authentications are required

Good sample text: The user needs to be logged in and have valid credentials to use this route.

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

This requests provides a HTML RESPONSE NUMBER on success.


This route is used to return a list of **only one** of the application sponsors (these are different than event sponsors).

=
#### Authentication

The user needs to be logged in and have valid credentials to use this route

=
#### Parameters

/:id

This is passed in the URL and is derived from the 'id' field on the the 'app_sponsors' table.

=
####JSON request example:
```
http://0.0.0.0:3000/app_sponsors/120
```
=
####JSON response example:

```
{"app_sponsor"=>
  {"id"=>120,
   "name"=>"Pouros Inc",
   "description"=>
    "Odio facilis vero in enim qui cumque vitae ut sequi distinctio autem.",
   "logo"=>nil,
   "url"=>nil,
   "sponsor_type"=>
    {"id"=>168, "name"=>"A type of Sponsor", "description"=>"A Sponsor Type"},
   "users"=>[]}}
```

This requests provides a <strong>HTML 200</strong> on success.