<!-- --- title: List of all parameters being used. -->

####URL Parameters

* (app_setting_option) :id - Integer, passed in the URL. Is derived from the 'id' field on the the 'app_setting_option' table.
* (event_bookmarks) :id - Integer, passed in the URL. Is derived from the 'id' field on the the 'event_bookmarks' table.
* (event_notes) :id - Integer, passed in through the URL. Is derived from the 'id' field of the 'event_notes' table.
* (event_user_schedules) :id - Integer, passed in through the URL. Is derived from the 'id' field of the 'event_user_schedules' table.
* (event_evaluations) :id - Integer, passed in through the URL. Is derived from the 'id' field of the 'event_evaluations' table.
* (event_session_evaluations) :id - Integer, passed in through the URL. Is derived from the 'id' field of the 'event_sessions_evaluations' table.
* (group_requests) :id - Integer, passed in the URL. Is derived from the 'id' field on the 'group_requests' table.
* (messages) :id - Integer, passed in through the URL. Is derived from the 'id' field of the 'messages' table.
* (post comment) :id - Integer, passed in through the URL. Is derived from the 'id' field on the 'post_comments' table.
* (post likes) :id - Integer, passed in through the URL. Is derived from the 'id' field on the 'post_likes' table.
* (post) :id - Integer, passed in through the URL. Is derived from the 'id' field on the 'posts' table.
* (post_comments) :id - Integer, passed in the URL. Is derived from the 'id' field on the 'post_comments' table.
* (post_likes) :id - Integer, passed in through the URL. Is derived from the 'id' field on the 'post_likes' table.
* (sponsor) :id - Integer, passed in through the URL. Is derived from the 'id' field on the the 'app_sponsors' table.
* :app_sponsor_id - Integer, passed in the URL. Is derived from the 'app_sponsor_id' field on the the 'banner_ads' table.
* :event_id - Integer, passed in through the URL. Is derived from the 'id' field of the 'events' table.
* :group_id - Integer, passed in through the URL. Is derived from the 'id' field on the 'groups' table.
* :group_invite_id - Integer, passed in through the URL. Is derived from the 'id' field on the 'group_invites' table.
* :group_members_id - Integer, passed in through the URL. Is derived from the 'id' field on the 'group_members' table.
* :group_requests_id - Integer, passed in the URL. Is derived from the 'id' field on the 'group_requests' table.
* :page - Text, passed in through the URL. Is derived from the 'name' field in the 'app_label_pages' table.
* :post_comments_id - Integer, passed in the URL. Is derived from the 'id' field on the 'post_comments' table.
* :post_id - Integer, passed in through the URL. Is derived from the 'id' field on the 'posts' table.
* :post_likes_id - Integer, passed in through the URL. Is derived from the 'id' field on the 'post_likes' table.
* :user_connection_id - Integer, passed in through the URL. Is derived from the 'id' field on the 'user_connection' table.
* :user_id - Integer, passed in through the URL. Is derived from the 'id' field on the 'users' table.

=
####Post data example: Parameters

* :alt_email - Varchar, passed in through the post data. Is derived from the 'alt_email' field on the 'users' table.
* :app_sponsor_id
* :bio  - Text, passed in through the post data. Is derived from the 'bio' field on the 'users' table. 
* :body - Text, passed in through the post data. This is the plain text of the submission.
* :body_markdown - Text, passed in through the post data. The formatted version of the post.
* :description - Text, passed in through the post data. Is derived from the 'description' field of the 'groups' table.
* :email - Varchar, passed in through the post data. If the user is not logged in, the app will ask the user for this, if they're logged in it will automatically fill it in.
* :event_id - Integer, passed in throug the post data. Is derived from the 'id' field on the 'events' table.
* :event_session_id - Integer, passed in through the post data. Is derived from the 'id' field on the 'event_sessions' table.
* :excerpt - Text, passed in through the post data. A synopsis of the post.
* :first_name - Varchar, passed in through the post data. Is derived from the 'first_name' field on the 'users' table.
* :group_id - Integer, passed in through the post data. Is derived from the 'id' field on the 'groups' table.
* :group_type_id - Integer, passed in through the post data. Is derived from the 'id' field on 'group_types' table.
* :last_name - Varchar, passed in through the post data. Is derived from the 'last_name' field on the 'users' table.
* :name - Varchar, passed in through the post data. Is derived from the 'name' field of the 'groups' table.
* :organization_name - Varchar, passed in through the post data. Is derived from the 'organization_name' field on the 'users' table. 
* :photo - Varchar, passed in through the post data. Is derived from the 'photo' field on the 'users' table.
* :post_id - Integer, passed in through the post data. Is derived from the 'id' field on the 'post' table.
* :recipient_user_id - Integer, passed in through the post data. This is 'user_id' of the person that is receiving the message. Derived from the 'id' field of the 'users' table'.
* :sender_user_id
* :thumbnail_teaser_photo - Varchar, passed in through the post data. The URL of a photo used to advertise the post
* :title - Text, passed in through the post data. The title of the post. Limited to 255 characters.
* :title - Varchar, passed in through the post data. Is derived from the 'title' field on the 'users' table.
* :user_id - Integer, passed in through the post data. Derived from the 'id' field of the 'users' table.