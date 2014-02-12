PLAIN ENGLISH DESCRIPTION OF THE ROUTE

Declare what authentications are required

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

This requests provides a HTML RESPONSE NUMBER on success and a HTML RESPONSE NUMBER ON FAILURE