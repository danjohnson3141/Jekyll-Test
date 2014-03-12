<!-- --- title: POST /users/password -->

This is the route used to begin the process of resetting a users password. The user sends submits an email address and the system then sends an email to that email address, the email will contain instructions on how the rest of the reset process should go.

=
#### Authentication

The user does not need to be logged in to use this route.

=
#### Parameters

:email - Varchar, passed in through the post data. Is derived from the 'email' field on the 'users' table. 

=
####JSON request example:
```json
http://0.0.0.0:3000/users/password
```

=
####JSON response example:

```json
NO JSON RESPONSE
```

This requests provides a <strong>HTML 201</strong> on success.