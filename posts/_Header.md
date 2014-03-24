* If an ‘event_session_post' record exists that references both a ‘post_id' and a ‘session_id’, then several * pieces of data are over-ridden in the API outputs because of this. 
* On Post related end points, the author data that would normally be derived from the ‘creator’ field on the * ‘posts’  table is instead being derived from the ‘speaker’ data on the ‘Sessions’ table.
* On Session related end points, the ‘name’ data that would normally be derived from the ‘name’ field on the * ‘Sessions’ table is instead being derived from the ‘title’ field on the ‘Posts’ table.
* On Session related end points, the ‘description’ data that would normally be derived from the * ‘description’ field on the ‘Sessions’ table is instead being derived from the ‘body’ field on the ‘Posts’ * table.
* The existense (or lack thereof) in no way impacts the behavior of the 'excerpt' on the post.
* [[flow_charts/post_visible.pdf]]