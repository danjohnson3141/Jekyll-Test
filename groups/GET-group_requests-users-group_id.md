<!-- --- title: GET /group_requests/users/:group_id -->

Returns a list of all the group requests for **one** group. Should not return any users who are members of the group. 

=
#### Authentication

The user needs to be logged in and have valid credentials to use this route.

=
#### Parameters

:group_id - Integer, passed in through the URL. Is derived from the 'id' field on the 'groups' table.

=
####JSON request example:
```json
http://stage-api-access.evant.com/group_requests/users/1917
```

=
####JSON response example:

```json
{"group_requests"=>
  [{"id"=>295,
    "group_id"=>1917,
    "user"=>
     {"id"=>15630,
      "email"=>"anthony.rowe@stokes.info",
      "alt_email"=>"tristian@gmail.com",
      "first_name"=>"Edna",
      "last_name"=>"Brakus",
      "title"=>"Random User",
      "organization_name"=>"D'Amore-Bechtelar",
      "bio"=>
       "Reiciendis sit possimus beatae est dicta culpa et vero facere totam ipsam.",
      "photo"=>
       "https://assets.evanta.com/shared/resources/Users/large/anonymous.jpg",
      "user_role_id"=>15632,
      "user_connection_id"=>nil}},
   {"id"=>294,
    "group_id"=>1917,
    "user"=>
     {"id"=>15627,
      "email"=>"willa@heaney.info",
      "alt_email"=>"pearlie_reynolds@yahoo.com",
      "first_name"=>"Jeromy",
      "last_name"=>"Huels",
      "title"=>"Random User",
      "organization_name"=>"Schroeder, Kreiger and Wilkinson",
      "bio"=>
       "Odit nostrum iste delectus doloribus est occaecati eum nisi ullam.",
      "photo"=>
       "https://assets.evanta.com/shared/resources/Users/large/anonymous.jpg",
      "user_role_id"=>15629,
      "user_connection_id"=>nil}}]}
```

This requests provides a <strong>HTML 200</strong> on success.