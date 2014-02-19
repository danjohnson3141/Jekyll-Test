List of all parameters being used.

=
####URL Parameters

* :app_sponsor_id - Integer, passed in the URL. Is derived from the 'app_sponsor_id' field on the the 'banner_ads' table.

* :event_id - Integer, passed in through the URL. Derived from the 'id' field of the 'events' table.

* :group_id - Integer, passed in through the URL. Is derived from the 'id' field on the 'groups' table.

* :page - Text, passed in through the URL. Each page of the App will have its own unique name. This parameter corresponds to the 'name' field in the app_label_pages table in the database.

* :post_id - Integer, passed in through the URL. Used to declare which post is going to be updated. It is derived from the 'id' field on the 'posts' table.

* (sponsor):id - Integer, passed in through the URL. Derived from the 'id' field on the the 'app_sponsors' table.

=
####Post Data Parameters

* :alt_email

* :app_sponsor_id

* :bio

* :body - Text, passed in through the post data. This is the plain text of the submission.

* :body_markdown - Text, passed in through the post data. The formatted version of the post.

* :description

* :email - Varchar, passed in through the post data. If the user is not logged in, the app will ask the user for this, if they're logged in it will automatically fill it in.

* :event_id

* :excerpt - Text, passed in through the post data. A synopsis of the post.

* :first_name

* :group_id

* :group_id - Integer, passed in through the post data. This is the 'id' of the group that the post will be associated with; derived from the 'id' field on the 'groups' table.

* :last_name

* :name

* :organization_name


* :photo

* :recipient_user_id

* :sender_user_id

* :thumbnail_teaser_photo - Varchar, passed in through the post data. The URL of a photo used to advertise the post

* :title - Text, passed in through the post data. The title of the post. Limited to 255 characters.

* :user_id