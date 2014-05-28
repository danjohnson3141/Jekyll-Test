<!-- --- title: GET /app_setting_options/:id -->

This returns the true or false value for one specifc application setting. Application settings are referenced by a

=
####Authentication:

The user needs to be logged in and have valid credentials to use this route.

=
####Parameters:

:name - Varchar, passed in through the URL.

=
####API request example:
```html
http://stage-api-access.evant.com/app_setting_options/text
```

=
####JSON response example:

```json
{"json_example"=>
  [{"id"=>123,
    "field1"=>"Text",
    "field2"=>nil
  }]
}
```

This requests provides a <strong>HTML 200</strong> on success.