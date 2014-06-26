<!-- --- title: PATCH /notifications/:id -->

This route is what changes notifications from being 'unread' to being 'read' [is_viewed from 0 to 1].

=
####Authentication:

The user needs to be logged in and have valid credentials to use this route.

=
####Parameters:

:id (notification) - Integer, passed in through the URL. Is derived from the 'id' field on the 'notifications' table.

=
####Response:

This requests provides a <strong>HTML 204</strong> on success.

=
####API request example:
```html
http://example.com/notifications/723
```

=
####Post data example:

NO POST DATA
 
=
###Post data detail:

NO POST DATA