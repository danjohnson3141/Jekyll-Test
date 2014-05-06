<!-- --- title: GET /post_followers/posts/:user_id -->

Featured posts are a list of posts that the application displays at the top of several pages (user feed, group feed, event feed). There is maximum number of posts that will be returned by this route. However, it is possible to artificially limit the number of posts returned through a suffix on the route. 

=
#### Authentication

Declare what authentications are required
Good sample text: The user needs to be logged in and have valid credentials to use this route.

=
#### Parameters

LIST OF ALL PARAMETERS AND WHAT THEY ARE

=
####JSON request example:
```json
http://0.0.0.0:3000/ROUTE_NAME
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

This requests provides a <strong>HTML RESPONSE NUMBER</strong> on success.