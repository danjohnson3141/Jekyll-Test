<!-- --- title: DELETE /event_followers/:id -->

Removes **one** event_follower record from the database. This is how a user unfollows an events. The active user is only able to remove records for which they are the follower, being the creator doesn't matter for this route.

=
####Authentication:

The user needs to be logged in and have valid credentials to use this route.

=
####Parameters:

:id - Integer, passed in through the URL. Is derived from the 'id' field on the 'event_followers' table.

=
####Response:

This requests provides a <strong>HTML 204</strong> on success.

=
####API request example:
```html
http://example.com/event_followers/234
```

=
####JSON response example:

[[include:/json/JSON_NO_RESPONSE]]