<!-- --- title: GET /banner_ads/groups/:group_id -->

This route requests all of the banner ads associated with a specific group.

=
#### Authentication
The user needs to be logged in and have valid credentials to use this route.

=
#### Parameters
:group_id

This is passed in the URL and is derived from the 'group_id' field on the the 'banner_ads' table.

=
####JSON request example:
```
http://0.0.0.0:3000/banner_ads/groups/3074
```

=
####JSON response example:

```
{"banner_ads"=>
  [{"id"=>285,
    "graphic_link"=>"www.example.com/graphic_link.jpg",
    "app_sponsor_id"=>nil,
    "link_url"=>"www.example.com",
    "created_by"=>nil,
    "updated_by"=>nil,
    "group"=>
     {"id"=>3074,
      "name"=>"Sleek Concrete Shirt",
      "description"=>
       "Temporibus soluta modi officiis accusantium laboriosam dolor.",
      "owner_user_id"=>nil,
      "app_sponsor_id"=>nil,
      "group_type"=>
       {"id"=>6435, "name"=>"Factory:Open", "description"=>"Open"},
      "owner"=>nil},
    "event"=>nil,
    "event_sponsor"=>nil,
    "app_sponsor"=>nil},
   {"id"=>286,
    "graphic_link"=>"www.example.com/graphic_link.jpg",
    "app_sponsor_id"=>nil,
    "link_url"=>"www.example.com",
    "created_by"=>nil,
    "updated_by"=>nil,
    "group"=>
     {"id"=>3074,
      "name"=>"Sleek Concrete Shirt",
      "description"=>
       "Temporibus soluta modi officiis accusantium laboriosam dolor.",
      "owner_user_id"=>nil,
      "app_sponsor_id"=>nil,
      "group_type"=>
       {"id"=>6435, "name"=>"Factory:Open", "description"=>"Open"},
      "owner"=>nil},
    "event"=>nil,
    "event_sponsor"=>nil,
    "app_sponsor"=>nil}]}
```

This requests provides a <strong>HTML 200</strong> on success.