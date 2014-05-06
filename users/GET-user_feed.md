<!-- --- title: GET /user_feed-->

This route is a collection of post and notifications that is specific to the active user. This list is procedurally generated based off of a variety of criteria. 


Feed is composed of:

* Posts in groups that the active user is a member of
* Posts in events that the active user is an event user of
* Visible posts that are commented on by connected user
* Visible posts that are liked by connected user
* Visible posts that are created by connected user
* Notifciation if connected user changes their title
* Notification is connected user changes their organization
* Posts the user is following

These items are sorted by the most recently created at the top of the list and then descending. Several actions that can be taken by other users can bump the order of the posts. These actions need to be taken by user connections of the active user for them to affect the user feed sort order. The exact same action taken by somebody who is not a connection will not affect the sort order.

* Comment on a visible post
* Like on a visible post
* Adding an attachment

If a user is following a post the above actions will also affect the sort order of that post regardless of the connection status of the user who perfomed that action.

=
#### Authentication

The user needs to be logged in and have valid credentials to use this route.

=
#### Parameters

none; default only

=
####JSON request example:
```json
http://0.0.0.0:3000/user_feed
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