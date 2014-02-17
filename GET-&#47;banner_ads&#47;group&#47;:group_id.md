This request returns all of the banner ads association with **one** group.

=
#### Authentication

The user needs to be logged in and have valid credentials to use this route.

=
#### Parameters

:group_id

This is derived from the 'id' field on the 'groups' table.

=
####JSON request example:
```
http://0.0.0.0:3000/banner_ads/group/895
```

=
####JSON response example:

```
{"banner_ads"=>
  [{"id"=>118,
    "graphic_link"=>"www.example.com/graphic_link.jpg",
    "app_sponsor_id"=>nil,
    "link_url"=>"www.example.com",
    "created_by"=>nil,
    "updated_by"=>nil,
    "group"=>
     {"id"=>895,
      "name"=>"Practical Wooden Pants",
      "description"=>
       "Sed quaerat iusto sed similique corporis quas quia nihil odit.",
      "owner_user_id"=>nil,
      "app_sponsor_id"=>nil,
      "group_type"=>
       {"id"=>1903, "name"=>"Factory:Open", "description"=>"Open"},
      "owner"=>nil},
    "event"=>nil,
    "event_sponsor"=>nil,
    "app_sponsor"=>nil},
   {"id"=>119,
    "graphic_link"=>"www.example.com/graphic_link.jpg",
    "app_sponsor_id"=>nil,
    "link_url"=>"www.example.com",
    "created_by"=>nil,
    "updated_by"=>nil,
    "group"=>
     {"id"=>895,
      "name"=>"Practical Wooden Pants",
      "description"=>
       "Sed quaerat iusto sed similique corporis quas quia nihil odit.",
      "owner_user_id"=>nil,
      "app_sponsor_id"=>nil,
      "group_type"=>
       {"id"=>1903, "name"=>"Factory:Open", "description"=>"Open"},
      "owner"=>nil},
    "event"=>nil,
    "event_sponsor"=>nil,
    "app_sponsor"=>nil}]}
```

This requests provides a <strong>HTML 200</strong> on success.