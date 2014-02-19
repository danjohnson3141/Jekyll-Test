List of all parameters being used.

=
####URL Parameters

* :event_id - Integer, passed in through the URL. Derived from the 'id' field of the 'events' table.

* :page - Text, passed in through the URL. Each page of the App will have its own unique name. This parameter corresponds to the 'name' field in the app_label_pages table in the database.

* :post_id - Integer, passed in through the URL. Used to declare which post is going to be updated. It is derived from the 'id' field on the 'posts' table.

* (sponsor):id - Integer, passed in through the URL. Derived from the 'id' field on the the 'app_sponsors' table.

=
####Post Data Parameters

* :alt_email

* :app_sponsor_id

* :bio

* :body - Text, passed in through the post data. The plain text of the post.

* :body_markdown - Text, passed in through the post data. The formatted version of the post.

* :description

* :email

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