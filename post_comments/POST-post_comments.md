<!-- --- title: POST /post_comments -->

This the method by which the active user ads a comment to an already existing post.

=
####Authentication:

The user needs to be logged in and have valid credentials to use this route.

=
####Parameters:

None; default ony.

=
####API request example:
```html
http://example.com/post_comments
```

=
####Post data example:
```
{ post_comment: 
  { body: 'Awesome post dude!', 
    post_id: 1053 } }
```
 
=
####JSON response example:

[[include:/json/JSON_POST_post_comments]]

=
####Response Data Detail:

[[include:/serializers/EXAMPLE]]