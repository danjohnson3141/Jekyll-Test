<!-- --- title: List of all routes -->

####App & Navigation
* [[DELETE /app_settings/:id|DELETE-app_settings-id]]
* [[GET /app_setting_options/:id|GET-app_setting_options-id]]
* [[GET /navigation/left|GET-navigation-left]]
* [[GET /navigation/right/:event_id|GET-navigation-right-event_id]]
* [[POST /app_settings|POST-app_settings]]
* [[POST /app_supports|POST-app_supports]]
* [[GET /app_labels/app|GET-app_labels-app]]
* [[GET /app_labels/event/:event_id|GET-app_labels-event-event_id]]
* [[GET /users/industry_type_options|GET-users-industry_type_options]]
* [[GET /users/region_options|GET-users-region_options]]
* [[GET /app_settings|GET-app_settings]]

=
####Event Bookmarks
* [[DELETE /event_bookmarks/:id|DELETE-event_bookmarks-id]]
* [[GET /event_bookmarks/event/:event_id|GET-event_bookmarks-event-event_id]]
* [[POST /event_bookmarks|POST-event_bookmarks]]

=
####Event Council
* [[GET /event_council_members/event/:event_id|GET-event_council_members-event-event_id]]

=
####Event Leaderboard
* [[GET /event_leaderboards/event/:event_id|GET-event_leaderboards-event-event_id]]
* [[GET /event_user_leaderboards/event/:event_id|GET-event_user_leaderboards-event-event_id]]

=
####Event Notes
* [[DELETE /event_notes/:id|DELETE-event_notes-id]]
* [[GET /event_notes/:id|GET-event_notes-id]]
* [[GET /event_notes/event/:event_id|GET-event_notes-event-event_id]]
* [[PATCH /event_notes/:id|PATCH-event_notes-id]]
* [[POST /event_notes|POST-event_notes]]
* [[PUT /event_notes/:id|PUT-event_notes-id]]

=
####Events
* [[DELETE /event_followers/:id|DELETE-event_followers-id]]
* [[DELETE /event_user_schedules/:id|DELETE-event_user_schedules-id]]
* [[DELETE /event_users/:id|DELETE-event_users-id]]
* [[GET /event_evaluations/:id|GET-event_evaluations-id]]
* [[GET /event_session_evaluations/:id|GET-event_session_evaluations-id]]
* [[GET /event_sessions/:id|GET-event_sessions-id]]
* [[GET /event_sessions/event/:event_id|GET-event_sessions-event-event_id]]
* [[GET /event_sessions/my_schedule/:event_id|GET-event_sessions-my_schedule-event_id]]
* [[GET /event_speakers/:id|GET-event_speakers-id]]
* [[GET /event_speakers/event/:event_id|GET-event_speakers-event-event_id]]
* [[GET /event_speakers/event_session/:event_session_id|GET-event_speakers-event_session-event_session_id]]
* [[GET /event_users/:id|GET-event_users-id]]
* [[GET /event_users/attendees/:event_id|GET-event_users-attendees-event_id]]
* [[GET /event_users/events/:user_id|GET-event_users-events-user_id]]
* [[GET /event_users/users/:event_id|GET-event_users-users-event_id]]
* [[GET /events/:id|GET-events-id]]
* [[GET /events/all|GET-events-all]]
* [[GET /events/past|GET-events-past]]
* [[GET /events/upcoming|GET-events-upcoming]]
* [[POST /event_followers|POST-event_followers]]
* [[POST /event_user_schedules|POST-event_user_schedules]]
* [[POST /event_users|POST-event_users]]

=
####Featured Posts
* [[GET /featured_posts/event/:event_id|GET-featured_posts-event-event_id]]
* [[GET /featured_posts/group/:group_id|GET-featured_posts-group-group_id]]
* [[GET /featured_posts/user|GET-featured_posts-user]]

=
####Groups
* [[DELETE /group_invites/:id|DELETE-group_invites-id]]
* [[DELETE /group_members/:id|DELETE-group_members-id]]
* [[DELETE /group_requests/:id|DELETE-group_requests-id]]
* [[GET /group_invites/groups|GET-group_invites-groups]]
* [[GET /group_invites/user_search/:group_id|GET-group_invites-user_search-group_id]]
* [[GET /group_invites/users/:group_id|GET-group_invites-users-group_id]]
* [[GET /group_members/groups/:user_id|GET-group_members-groups-user_id]]
* [[GET /group_members/users/:group_id|GET-group_members-users-group_id]]
* [[GET /group_requests/groups|GET-group_requests-groups]]
* [[GET /group_requests/users/:group_id|GET-group_requests-users-group_id]]
* [[GET /groups/:id|GET-groups-id]]
* [[GET /groups|GET-groups]]
* [[PATCH /group_requests/:id|PATCH-group_requests-id]]
* [[PATCH /groups/:id|PATCH-groups-id]]
* [[POST /group_invites|POST-group_invites]]
* [[POST /group_members|POST-group_members]]
* [[POST /group_requests|POST-group_requests]]
* [[POST /groups|POST-groups]]
* [[PUT /group_requests/:id|PUT-group_requests-id]]
* [[PUT /groups/:id|PUT-groups-group_id]]

=
####Messages
* [[DELETE /messages/:id|DELETE-messages-message_id]]
* [[DELETE /messages/conversation/:user_id|DELETE-messages-conversation-user_id]]
* [[GET /messages/conversation/:user_id|GET-messages-conversation-user_id]]
* [[GET /messages|GET-messages]]
* [[POST /messages|POST-messages]]
* [[GET /messages/user_search/:query|GET-messages-user_search-query]]

=
####Notifications
* [[GET /notifications|GET-notifications]]
* [[PATCH /notifications/:id|PATCH-notifications-id]]
* [[PUT /notifications/:id|PUT-notifications-id]]

=
####Post Attachments
* [[DELETE /post_attachments/:id|DELETE-post_attachments-id]]
* [[POST /post_attachments|POST-post_attachments]]

=
####Post Comments
* [[DELETE /post_comments/:id|DELETE-post_comments-id]]
* [[GET /post_comments/post/:post_id|GET-post_comments-post-id]]
* [[PATCH /post_comments/:id|PATCH-post_comments-id]]
* [[POST /post_comments|POST-post_comments]]
* [[PUT /post_comments/:id|PUT-post_comments-id]]

####Post Likes
* [[DELETE /post_likes/:id|DELETE-post_likes-id]]
* [[GET /post_likes/:id|GET-post_likes-id]]
* [[GET /post_likes/posts/:user_id|GET-post_likes-post-id]]
* [[GET /post_likes/users/:post_id|GET-post_likes-user-id]]
* [[POST /post_likes|POST-post_likes]]

=
####Posts
* [[POST /post_followers|POST-post_followers]]
* [[GET /post_followers/users/:post_id|GET-post_followers-users-post_id]]
* [[GET /post_followers/posts/:user_id|GET-post_followers-posts-user_id]]
* [[DELETE /post_followers/:id|DELETE-post_followers-id]]
* [[DELETE /posts/:id|DELETE-posts-post_id]]
* [[GET /posts/:id|GET-posts-post_id]]
* [[GET /posts/event/:event_id|GET-posts-events-id]]
* [[GET /posts/group/:group_id|GET-posts-groups-group_id]]
* [[GET /posts/user/:user_id|GET-posts-users-user_id]]
* [[PATCH /posts/:id|PATCH-posts-post_id]]
* [[POST /posts|POST-posts]]
* [[PUT /posts/:id|PUT-posts-post_id]]
* [[GET /posts/similar/:post_id|GET-posts-similar-post_id]]
* [[GET /posts/sponsor/:sponsor_id|GET-posts-sponsor-sponsor_id]]

=
####Search
* [[GET /search/content|GET-search-content]]
* [[GET /search/event_groups|GET-search-event_groups]]
* [[GET /search/users|GET-search-users]]

=
####Sponsors
* [[GET /sponsors/:id|GET-sponsors-id]]
* [[GET /sponsors/app|GET-sponsors-app]]
* [[GET /sponsors/event|GET-sponsors-event]]
* [[GET /sponsors/group|GET-sponsors-group]]
* [[GET /sponsors|GET-sponsors]]
* [[GET /sponsors/homepage|GET-sponsors-homepage]]

=
####User Connections
* [[DELETE /user_connections/:id|DELETE-user_connections-id]]
* [[GET /user_connections/pending|GET-user_connections-pending]]
* [[PATCH /user_connections/:id|PATCH-user_connections-user_connection_id]]
* [[POST /user_connections|POST-user_connections]]
* [[PUT /user_connections/:id|PUT-user_connections-user_connection_id]]
* [[GET /user_connections/user/:user_id|GET-user_connections-user-user_id]]

=
####Users
* [[GET /users/settings|GET-users-settings]]
* [[GET /users/locale_options|GET-users-locale_options]]
* [[GET /user_feed|GET-user_feed]]
* [[DELETE /users/sign_out|DELETE-users-sign_out]]
* [[GET /users/profile|GET-users-profile]]
* [[PATCH /users/password|PATCH-users-password]]
* [[PATCH /users/profile|PATCH-users-profile]]
* [[POST /users/password|POST-users-password]]
* [[POST /users/sign_in|POST-users-sign_in]]
* [[PUT /users/password|PUT-users-password]]
* [[PUT /users/profile|PUT-users-profile]]
* [[GET /users/post_options|GET-users-post_options]]
* [[GET /users/profile/:user_id|GET-users-profile-user_id]]

=
####Routes that exist, but not really
These exist just so that documentation audits don't get tripped up:

* GET /users/password/edit
* GET /users/password/new
* GET /users/sign_in
* OPTIONS /*path

These routes are used internally only:

* DELETE /sync/event_sessions/:client_id
* DELETE /sync/events/:client_id
* DELETE /sync/sponsors/:client_id
* GET /sync/event_sessions/:client_id
* GET /sync/events/:client_id
* GET /sync/sponsors/:client_id
* PATCH /sync/event_sessions/:client_id
* PATCH /sync/events/:client_id
* PATCH /sync/sponsors/:client_id
* POST /sync/event_sessions
* POST /sync/events
* POST /sync/sponsors
* PUT /sync/event_sessions/:client_id
* PUT /sync/events/:client_id
* PUT /sync/sponsors/:client_id