<!-- --- title: PUT /posts/:id -->

This updates records in the 'posts' table.

=
####Authentication:

The user needs to be logged in and have valid credentials to use this route.

=
####Parameters:

:post_id - Integer, passed in through the URL. Used to declare which post is going to be updated. It is derived from the 'id' field on the 'posts' table.

:title - Text, passed in through the post data. The title of the post. Limited to 255 characters.

:body - Text, passed in through the post data. The plain text of the post.

:body_markdown - Text, passed in through the post data. The formatted version of the post.

:excerpt - Text, passed in through the post data. A synopsis of the post.

:thumbnail_teaser_photo - Varchar, passed in through the post data. The URL of a photo used to advertise the post

=
####JSON request example
```
http://example.com/posts/234
```

=
####Post data example:
```
{ post: 
  { title: "Coffee Pot", 
    body: "A covered container with a spout, in which coffee is made or served.", 
    body_markdown: "A **covered** *container* with a spout, in which coffee is made or served.",
    excerpt: "covered container",
    thumbnail_teaser_photo: "www.example.com/new_photo.png"} 
  }
```

=
####JSON response example:

[[include:/json/JSON_NO_RESPONSE]]

This requests provides a <strong>HTML 204</strong> on success.