<!-- --- title: GET /posts/events/:event_id -->

Returns **all** of the posts associated with **one** event.

=
#### Authentication

The user needs to be logged in and have valid credentials to use this route.

=
#### Parameters

:event_id - Integer, passed in through the URL. Is derived from the 'id' field of the 'events' table.


=
####JSON request example:
```json
http://0.0.0.0:3000/posts/events/5803
```

=
####JSON response example:

```json
{"posts"=>
  [{"id"=>2621,
    "title"=>nil,
    "excerpt"=>nil,
    "thumbnail_teaser_photo"=>nil,
    "view_count"=>nil,
    "show_likes_count"=>true,
    "like_count"=>0,
    "comment_count"=>0,
    "post_like_id"=>nil,
    "post_likes"=>true,
    "show_post_likes_list"=>true,
    "post_attachments"=>[],
    "authors"=>[nil],
    "ago"=>"0m",
    "group"=>nil,
    "event"=>{"id"=>5803, "name"=>"Practical Cotton Computer 371"}},
   {"id"=>2622,
    "title"=>nil,
    "excerpt"=>nil,
    "thumbnail_teaser_photo"=>nil,
    "view_count"=>nil,
    "show_likes_count"=>true,
    "like_count"=>0,
    "comment_count"=>0,
    "post_like_id"=>nil,
    "post_likes"=>true,
    "show_post_likes_list"=>true,
    "post_attachments"=>[],
    "authors"=>[nil],
    "ago"=>"0m",
    "group"=>nil,
    "event"=>{"id"=>5803, "name"=>"Practical Cotton Computer 371"}},
   {"id"=>2623,
    "title"=>nil,
    "excerpt"=>nil,
    "thumbnail_teaser_photo"=>nil,
    "view_count"=>nil,
    "show_likes_count"=>true,
    "like_count"=>0,
    "comment_count"=>0,
    "post_like_id"=>nil,
    "post_likes"=>true,
    "show_post_likes_list"=>true,
    "post_attachments"=>[],
    "authors"=>[nil],
    "ago"=>"0m",
    "group"=>nil,
    "event"=>{"id"=>5803, "name"=>"Practical Cotton Computer 371"}},
   {"id"=>2624,
    "title"=>nil,
    "excerpt"=>nil,
    "thumbnail_teaser_photo"=>nil,
    "view_count"=>nil,
    "show_likes_count"=>true,
    "like_count"=>0,
    "comment_count"=>0,
    "post_like_id"=>nil,
    "post_likes"=>true,
    "show_post_likes_list"=>true,
    "post_attachments"=>[],
    "authors"=>[nil],
    "ago"=>"0m",
    "group"=>nil,
    "event"=>{"id"=>5803, "name"=>"Practical Cotton Computer 371"}},
   {"id"=>2625,
    "title"=>nil,
    "excerpt"=>nil,
    "thumbnail_teaser_photo"=>nil,
    "view_count"=>nil,
    "show_likes_count"=>true,
    "like_count"=>0,
    "comment_count"=>0,
    "post_like_id"=>nil,
    "post_likes"=>true,
    "show_post_likes_list"=>true,
    "post_attachments"=>[],
    "authors"=>[nil],
    "ago"=>"0m",
    "group"=>nil,
    "event"=>{"id"=>5803, "name"=>"Practical Cotton Computer 371"}}]}
```

This requests provides a <strong>HTML RESPONSE NUMBER</strong> on success.