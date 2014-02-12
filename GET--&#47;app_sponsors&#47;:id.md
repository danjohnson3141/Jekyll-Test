This route is used to return a list of **only one** of the application sponsors (these are different than event sponsors).

The user needs to be logged in and have valid credentials to use this route

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

This requests provides a HTML 200 on success.