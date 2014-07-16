<!-- --- title: GET /sponsors/homepage -->

Returns a list of **all** sponsors that have a value of '1' in the homepage_sponsor field on the sponsors table. Current business logic says that there should only ever be one of these, but there's nothing procedurally requiring that.

=
####Authentication:

The user does not need to be authenticated to use this route.

=
####Parameters:

None; default only.

=
####Response:

This requests provides a <strong>HTML 200</strong> on success.

=
####API request example:
```html
http://example.com/sponsors/homepage
```

=
####JSON response example:

[[include:/json/JSON_GET_sponsors_homepage]]

=
####Response Data Detail:

[[include:/serializers/sponsor_tiny]]