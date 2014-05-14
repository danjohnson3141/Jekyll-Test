<!-- --- title: POST /post_comments -->

This the method by which the active user ads a comment to an already existing post.

=
#### Authentication

The user needs to be logged in and have valid credentials to use this route.

=
#### Parameters

:body - Text, passed in through the post data. This is the plain text of the submission.
:post_id - Integer, passed in through the post data. Is derived from the 'id' field on the 'post' table.


=
####API request example:
```json
http://stage-api-access.evant.com/post_comments
```

=
###Post Data:
```json
{ post_comment: { body: 'Awesome post dude!', post_id: 1053 } }
```

=
####JSON response example:

```json
{"post_comment"=>
  {"id"=>10,
   "body"=>"Awesome post dude!",
   "ago"=>"0m",
   "post_id"=>4,
   "creator"=>
    {"id"=>1,
     "first_name"=>"Generic",
     "last_name"=>"User",
     "title"=>"CEO of QA",
     "organization_name"=>"Evanta",
     "photo"=>
      "https://assets.evanta.com/shared/resources/Users/large/anonymous2.jpg",
     "moderator"=>false,
     "user_profile"=>true}}}
```

This requests provides a <strong>HTML 201</strong> on success.