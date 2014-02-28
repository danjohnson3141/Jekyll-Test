####App & Navigation
* [[GET /app/labels/:page]] 
* [[GET /app_setting_options/:id]] 
* [[GET /app_settings/:name]] 
* [[GET /app_sponsors/:app_sponsor_id]] 
* [[GET /app_sponsors]] 
* [[POST /app_supports]] 
* [[GET /navigation/left]] 
* [[GET /navigation/right/:event_id]] 

=
####Banner Ads
* [[GET /banner_ads/app_sponsor/:app_sponsor_id]] 
* [[GET /banner_ads/event/:event_id]] 
* [[GET /banner_ads/group/:group_id]] 
* [[GET /banner_ads]] 

=
####Events
* [[GET /event_featured_posts/:event_id]] 
* [[DELETE /event_followers/:id]] 
* [[GET /event_followers/events/:user_id]] 
* [[GET /event_followers/users/:event_id]] 
* [[POST /event_followers]] 
* [[GET /event_sessions/:event_session_id]] 
* [[GET /event_sessions/events/:event_id]] 
* [[GET /event_sponsors/:id]] 
* [[GET /event_sponsors]] 
* [[DELETE /event_users/:id]] 
* [[GET /event_users/attendees/:event_id]] 
* [[GET /event_users/events/:user_id]] 
* [[GET /event_users/users/:event_id]] 
* [[POST /event_users]] 
* [[GET /events/:event_id]] 
* [[GET /events/all/:user_id]] 
* [[GET /events/all]] 
* [[GET /events/past/:user_id]] 
* [[GET /events/past]] 
* [[GET /events/upcoming/:user_id]] 
* [[GET /events/upcoming]] 
* [[GET /events]] 

=
####Groups
* [[GET /group_featured_posts/:group_id]] 
* [[DELETE /group_invites/:id]] 
* [[GET /group_invites/groups]] 
* [[GET /group_invites/users/:group_id]] 
* [[POST /group_invites]] 
* [[DELETE /group_members/:id]] 
* [[GET /group_members/groups/:user_id]] 
* [[GET /group_members/users/:group_id]] 
* [[POST /group_members]] 
* [[DELETE /group_requests/:id]] 
* [[GET /group_requests/groups]] 
* [[GET /group_requests/users/:group_id]] 
* [[POST /group_requests]] 
* [[GET /groups/:id]] 
* [[PATCH /groups/:id]] 
* [[PUT /groups/:id]] 
* [[GET /groups]] 
* [[POST /groups]] 

=
####Messages
* [[DELETE /messages/:id]] 
* [[GET /messages/conversation/:user_id]] 
* [[GET /messages]] 
* [[POST /messages]] 

=
####Posts
* [[DELETE /posts/:post_id]] 
* [[GET /posts/:post_id]] 
* [[PATCH /posts/:post_id]] 
* [[PUT /posts/:post_id]] 
* [[GET /posts/groups/:group_id]] 
* [[GET /posts/users/:user_id]] 
* [[POST /posts]] 

=
####Users
* [[DELETE /user_connections/:id]] 
* [[PATCH /user_connections/:id]] 
* [[PUT /user_connections/:id]] 
* [[GET /user_connections/:user_id]] 
* [[POST /user_connections]] 
* [[GET /users/password/edit]] 
* [[GET /users/password/new]] 
* [[PATCH /users/password]] 
* [[POST /users/password]] 
* [[PUT /users/password]] 
* [[GET /users/profile/:id]] 
* [[GET /users/profile]] 
* [[PATCH /users/profile]] 
* [[PUT /users/profile]] 
* [[GET /users/sign_in]] 
* [[POST /users/sign_in]] 
* [[DELETE /users/sign_out]] 
