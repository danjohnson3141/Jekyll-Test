<!-- --- title: List of all routes -->

####App & Navigation
* [[GET /app/labels/:page|GET-&#47app_sponsors]]
* [[GET /app_setting_options/:id|GET-&#47;app_setting_options&#47;:id]]
* [[GET /app_settings/:name|GET-&#47;app_settings&#47;:name]]
* [[GET /app_sponsors/:app_sponsor_id|GET-&#47;app_sponsors&#47;:app_sponsor_id]]
* [[GET /app_sponsors|GET-&#47;app_sponsors]]
* [[POST /app_supports|POST-&#47;app_supports]]
* [[GET /navigation/left|GET-&#47;navigation&#47;left]]
* [[GET /navigation/right/:event_id|GET-&#47;navigation&#47;right&#47;:event_id]]

=
####Banner Ads
* [[GET /banner_ads/app_sponsor/:app_sponsor_id|GET-&#47;banner_ads&#47;app_sponsor&#47;:app_sponsor_id]]
* [[GET /banner_ads/event/:event_id|GET-&#47;banner_ads&#47;event&#47;:event_id]]
* [[GET /banner_ads/group/:group_id|GET-&#47;banner_ads&#47;group&#47;:group_id]]
* [[GET /banner_ads|GET-&#47;banner_ads]]

=
####Events
* [[GET /event_featured_posts/:event_id|GET-&#47;event_featured_posts&#47;:event_id]]
* [[DELETE /event_followers/:id|DELETE-&#47;event_followers&#47;:id]]
* [[GET /event_followers/events/:user_id|GET-&#47;event_followers&#47;events&#47;:user_id]]
* [[GET /event_followers/users/:event_id|GET-&#47;event_followers&#47;users&#47;:event_id]]
* [[POST /event_followers|POST-&#47;event_followers]]
* [[GET /event_sessions/:event_session_id|GET-&#47;event_sessions&#47;:event_session_id]]
* [[GET /event_sessions/events/:event_id|GET-&#47;event_sessions&#47;events&#47;:event_id]]
* [[GET /event_sponsors/:id|GET-&#47;event_sponsors&#47;:event_sponsor_id]]
* [[GET /event_sponsors|GET-&#47;event_sponsors]]
* [[DELETE /event_users/:id|DELETE-&#47;event_users&#47;:id]]
* [[GET /event_users/attendees/:event_id|GET-&#47;event_users&#47;attendees&#47;:event_id]]
* [[GET /event_users/events/:user_id|GET-&#47;event_users&#47;events&#47;:user_id]]
* [[GET /event_users/users/:event_id|GET-&#47;event_users&#47;users&#47;:event_id]]
* [[POST /event_users|POST-&#47;event_users]]
* [[GET /events/:event_id|GET-&#47;events&#47;:event_id]]
* [[GET /events/all/:user_id|GET-&#47;events&#47;all&#47;:user_id]]
* [[GET /events/all|GET-&#47;events&#47;all]]
* [[GET /events/past/:user_id|GET-&#47;events&#47;past&#47;:user_id]]
* [[GET /events/past|GET-&#47;events&#47;past]]
* [[GET /events/upcoming/:user_id|GET-&#47;events&#47;upcoming&#47;:user_id]]
* [[GET /events/upcoming|GET-&#47;events&#47;upcoming]]
* [[GET /events|GET-&#47;events]]

=
####Groups
* [[GET /group_featured_posts/:group_id|GET-&#47;group_featured_posts&#47;:group_id]]
* [[DELETE /group_invites/:id|DELETE-&#47;group_invites&#47;:id]]
* [[GET /group_invites/groups|GET-&#47;group_invites&#47;groups]]
* [[GET /group_invites/users/:group_id|GET-&#47;group_invites&#47;users&#47;:group_id]]
* [[POST /group_invites|POST-&#47;group_invites]]
* [[DELETE /group_members/:id|DELETE-&#47;group_members&#47;:id]]
* [[GET /group_members/groups/:user_id|GET-&#47;group_members&#47;groups&#47;:user_id]]
* [[GET /group_members/users/:group_id|GET-&#47;group_members&#47;users&#47;:group_id]]
* [[POST /group_members|POST-&#47;group_members]]
* [[DELETE /group_requests/:id|DELETE-&#47;group_requests&#47;:id]]
* [[GET /group_requests/groups|GET-&#47;group_requests&#47;groups]]
* [[GET /group_requests/users/:group_id|GET-&#47;group_requests&#47;users&#47;:group_id]]
* [[POST /group_requests|POST-&#47;group_requests]]
* [[GET /groups/:id|GET-&#47;groups&#47;:id]]
* [[PATCH /groups/:id|PATCH-&#47;groups&#47;:id]]
* [[PUT /groups/:id|PUT-&#47;groups&#47;:id]]
* [[GET /groups|GET-&#47;groups]]
* [[POST /groups|POST-&#47;groups]]

=
####Messages
* [[DELETE /messages/:id|DELETE-&#47;messages&#47;:id]]
* [[GET /messages/conversation/:user_id|GET-&#47;messages&#47;conversation&#47;:user_id]]
* [[GET /messages|GET-&#47;messages]]
* [[POST /messages|POST-&#47;messages]]

=
####Posts
* [[DELETE /posts/:post_id|DELETE-&#47;posts&#47;:post_id]]
* [[GET /posts/:post_id|GET-&#47;posts&#47;:post_id]]
* [[PATCH /posts/:post_id|PATCH-&#47;posts&#47;:post_id]]
* [[PUT /posts/:post_id|PUT-&#47;posts&#47;:post_id]]
* [[GET /posts/groups/:group_id|GET-&#47;posts&#47;groups&#47;:group_id]]
* [[GET /posts/users/:user_id|GET-&#47;posts&#47;users&#47;:user_id]]
* [[POST /posts|POST-&#47;posts]]

=
####Users
* [[DELETE /user_connections/:id|DELETE-&#47;user_connections&#47;:id]]
* [[PATCH /user_connections/:id|PATCH-&#47;user_connections&#47;:id]]
* [[PUT /user_connections/:id|PUT-&#47;user_connections&#47;:id]]
* [[GET /user_connections/:user_id|GET-&#47;user_connections&#47;:user_id]]
* [[POST /user_connections|POST-&#47;user_connections]]
* [[GET /users/password/edit|GET-&#47;users&#47;password&#47;edit]]
* [[GET /users/password/new|GET-&#47;users&#47;password&#47;new]]
* [[PATCH /users/password|PATCH-&#47;users&#47;password]]
* [[POST /users/password|POST-&#47;users&#47;password]]
* [[PUT /users/password|PUT-&#47;users&#47;password]]
* [[GET /users/profile/:id|GET-&#47;users&#47;profile&#47;:id]]
* [[GET /users/profile|GET-&#47;users&#47;profile]]
* [[PATCH /users/profile|PATCH-&#47;users&#47;profile]]
* [[PUT /users/profile|PUT-&#47;users&#47;profile]]
* [[GET /users/sign_in|GET-&#47;users&#47;sign_in]]
* [[POST /users/sign_in|POST-&#47;users&#47;sign_in]]
* [[DELETE /users/sign_out|DELETE-&#47;users&#47;sign_out]]