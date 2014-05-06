<!-- --- title: GET /user_feed-->

This route is a collection of post and notifications that is specific to the active user. This list is procedurally generated based off of a variety of criteria. 


Feed is composed of:

* Posts in groups that the active user is a member of
* Posts in events that the active user is an event user of
* Visible posts that are commented on by connected user
* Visible posts that are liked by connected user
* Visible posts that are created by connected user
* Notifciation if connected user changes their title
* Notification if connected user changes their organization
* Notification if connected user registers for visible and/or followed event
* Notification if connected user creates a visible group
* Posts the user is following

These items are sorted by the most recently created at the top of the list and then descending. Several actions that can be taken by other users can affect the order of the posts by bumping tht post to the top of the list. Whether or not the user is following a post and also whether the action was taken by a connection or non-connection will affect this. If the user *is not* following the post, the action must be taken by a connection for it to affect the sort order. If the user *is* following the post, then the action does not need to be performed by a connection for the sort order to be affected.

* Comment on a visible post
* Like on a visible post
* Adding an attachment

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