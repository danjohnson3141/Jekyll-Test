<!-- --- title: GET /navigation/leftw -->

This is a route to help populate the left navigation element in the app (e.g. clicking on the bug).

The user needs to be logged in and have valid credentials to use this route.

#### Parameters

This route has no parameters and returns its content based on the users's internal settings.

=
####JSON request example:
```
http://0.0.0.0:3000/navigation/left
```
=
####JSON response example:

```
{"navigation_left"=>
  {"show_messages"=>true,
   "show_notifications"=>false,
   "show_search"=>false,
   "show_user_profile"=>false,
   "show_posts_count"=>false,
   "show_likes_count"=>false,
   "show_connections_count"=>false,
   "show_groups"=>false,
   "show_events"=>false,
   "show_app_sponsors"=>true,
   "show_support_link"=>true,
   "new_message_count"=>0,
   "new_notification_count"=>nil,
   "user_headshot"=>nil,
   "user_full_name"=>nil,
   "user_title"=>nil,
   "user_organization"=>nil,
   "user_post_count"=>nil,
   "user_like_count"=>nil,
   "user_connection_count"=>nil,
   "user_events"=>[],
   "user_today_events"=>nil,
   "user_groups"=>[]}}
```

This requests provides a HTML 200 on success.