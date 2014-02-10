This route is used to populate the various text form elements on each page. The database groups these into 'dictionaries' for each page of the application and returns all the labels for that page rather than having the API ask for each label individually. 

=
### Parameters

/:page

This is passed in through the URL. Each page of the App will have its own unique name.

=


JSON response example:

```
{"app_label_pages"=>
  [{"id"=>10,
    "key"=>"Test Dictionary",
    "label"=>"Testing Label Text",
    "label_plural"=>nil}]}
```

This request should provide a 200 HTTP response when successful and a 404 when it fails.