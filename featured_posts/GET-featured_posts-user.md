<!-- --- title: GET /featured_posts/user -->

Featured posts are a list of posts that the application displays at the top of several pages (currently: user feed, group feed, event feed). There is no maximum number of posts that will be returned by this route. However, it is possible to artificially limit the number of posts returned through a suffix on the route, which is: '?limit=X' where X is the number to return.

The database table that manages this route only has two relevant fields that are addressed by the application, they are 'post_id' and 'created_at'. The post_id is just the reference to the post that should appear in the feed, created_at is only relevant for purposes of sorting the list.

The user route (as opposed to event and group routes) is composed of all the featured group posts from groups that the active user is a member of.

=
####Authentication:

The user needs to be logged in and have valid credentials to use this route.

=
####Parameters:

suffix: '?limit=X' 

=
####API request example:
```html
http://example.com/featured_posts/user?limit=5
```

=
####JSON response example:

[[include:/json/JSON_GET_featured_posts_user]]

=
####Response Data Detail:

[[include:/serializers/EXAMPLE]]