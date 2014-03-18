<!-- --- title: GET /app_settings/:name -->

This returns the true or false value for one specifc application setting. Application settings are referenced by a

=
#### Authentication

The user needs to be logged in and have valid credentials to use this route.

=
#### Parameters

:name - Varchar, passed in through the URL.

=
####JSON request example:
```json
http://0.0.0.0:3000/app_settings/text
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