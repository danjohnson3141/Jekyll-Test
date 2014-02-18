S

=
#### Authentication

Declare what authentications are required

Good sample text: The user needs to be logged in and have valid credentials to use this route.

=
#### Parameters

:title - Text, passed in through the post data. The title of the post. Limited to 255 characters. 

:body - Text, passed in through the post data. The plain text of the post.

:body_markdown - Text, passed in through the post data. The formatted version of the post. 

:excerpt - Text, passed in through the post data. A synopsis of the post.

:thumbnail_teaser_photo - Varchar, passed in through the post data. The URL of a photo used to advertise the post

:group_id - Integer, passed in through the post data. This is the 'id' of the group that the post will be associated with; derived from the 'id' field on the 'groups' table.

=
####JSON request example:
```
http://0.0.0.0:3000/posts
```

=
####JSON response example:

```
{"json_example"=>
  [{"id"=>123,
    "field1"=>"Text",
    "field2"=>nil
  }]
}
```

This requests provides a <strong>HTML RESPONSE NUMBER</strong> on success.