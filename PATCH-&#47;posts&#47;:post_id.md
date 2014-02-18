This updates records in the 'posts' table.

=
#### Authentication

The user needs to be logged in and have valid credentials to use this route.

=
#### Parameters

:post_id

This references

=
####JSON request example
```
http://0.0.0.0:3000/posts/234
```

=
####Post Data
```
{ post: 
  { title: "Coffee Pot", 
    body: "A covered container with a spout, in which coffee is made or served.", 
    body_markdown: "A **covered** *container* with a spout, in which coffee is made or served.",
    excerpt: "covered container",
    thumbnail_teaser_photo: "www.example.com/new_photo.png"
    } 
  }
```

=
####JSON response example:

```
NO JSON RESPONSE
```

This requests provides a <strong>HTML 204</strong> on success.