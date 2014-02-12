This route is used to return a list of only one of the application sponsors (these are different than event sponsors).

Declare what authentications are required

#### Parameters

LIST OF ALL PARAMETERS AND WHAT THEY ARE

=
####JSON request example:
```
http://0.0.0.0:3000//app_sponsors/120
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
[3] pry(#<RSpec::Exa
```

This requests provides a HTML RESPONSE NUMBER on success and a HTML RESPONSE NUMBER ON FAILURE