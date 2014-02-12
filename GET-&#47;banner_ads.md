PLAIN ENGLISH DESCRIPTION OF THE ROUTE

Declare what authentications are required

Good sample text: The user needs to be logged in and have valid credentials to use this route.

#### Parameters

LIST OF ALL PARAMETERS AND WHAT THEY ARE

=
####JSON request example:
```
http://0.0.0.0:3000/ROUTE_NAME
```
=
####JSON response example:

```
{"banner_ads"=>
  [{"id"=>175,
    "graphic_link"=>"www.link.com/graphic_link.jpg",
    "app_sponsor_id"=>nil,
    "link_url"=>"www.evanta.com",
    "created_by"=>nil,
    "updated_by"=>nil,
    "group"=>nil,
    "event"=>nil,
    "event_sponsor"=>nil,
    "app_sponsor"=>nil},
   {"id"=>176,
    "graphic_link"=>"www.link.com/graphic_link.jpg",
    "app_sponsor_id"=>nil,
    "link_url"=>"www.evanta.com",
    "created_by"=>nil,
    "updated_by"=>nil,
    "group"=>nil,
    "event"=>nil,
    "event_sponsor"=>nil,
    "app_sponsor"=>nil}]}
```

This requests provides a HTML RESPONSE NUMBER on success and a HTML RESPONSE NUMBER ON FAILURE