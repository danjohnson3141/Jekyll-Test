<!-- --- GET /app_supports-->

This is the route used for the user to submit support requests to the application admins. 

=
#### Authentication

No authorizations required

=
#### Parameters

:body - Text, passed in through the post data. This is the plain text of the submission.

:email - Varchar, passed in through the post data. If the user is not logged in, the app will ask the user for this, if they're logged in it will automatically fill it in.

=
####JSON request example:
```
http://0.0.0.0:3000/app_supports
```

=
####POST Data
```
{ app_support: 
  {body: "I need help!!!", 
   email: "distraught_user@example.com"} 
 }
```
=
####JSON response example:

```
{"app_support"=>
  {"id"=>36,
   "body"=>"I need help!!!",
   "email"=>"distraught_user@example.com",
   "created_by_user"=>"Generic User"}}
```

This requests provides a <strong>HTML 201</strong> on success.