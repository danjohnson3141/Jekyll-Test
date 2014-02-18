This route is used to populate the various text form elements on each page. The database groups these into 'dictionaries' for each page of the application and returns all the labels for that page rather than having the API ask for each label individually. 

=
####Authentication

Some requests do not require the user to be authenticated, this is determined by the 'auth_required' field of the app_label_pages table in the database (0 = auth not required, 1 = auth required).

=
#### Parameters

/:page - Text, passed in through the URL. Each page of the App will have its own unique name. This parameter corresponds to the 'name' field in the app_label_pages table in the database.

=
####JSON request example:
```
http://0.0.0.0:3000/app/labels/login
```
=
####JSON response example:

```
{"app_label_pages"=>
  [{"id"=>10,
    "key"=>"Test Dictionary",
    "label"=>"Testing Label Text",
    "label_plural"=>nil}]}
```

This request should provide a <strong>200 HTTP</strong> response when successful.