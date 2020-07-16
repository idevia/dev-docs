# Getting or Posting data

To make our dev life easier we have decided to follow certain rules for getting and posting data.

## API endpoints

We use only 4 type of requests, **GET**, **POST**, **PUT** and **DELETE**, for **CRUD** operations. Suppose we are creating, fetching, updating and deleting **user**. So the endpoints should look like:

Create user:

?> **POST _/users/create_**

Get users:

?> **GET _/users_**

Get a single user:

?> **GET _/users/:id_**

Update a single user:

?> **PUT _/users/update_**

Update a single user:

?> **DEL _/users/:id_**

!> **Note:** URL segment must be plural.

## Request parameters

Request parameters are really important when you send data to the APIs that we build. We have set the following rules for this:

- camel casing not allowed
- You have to use snake-case (**request-param**)
- If you need to send the _id_ of any document, you'll be sending **id**, not **_\_id_**, **_userId_** or **_user_id_**

!> **Note:** camel casing is not allowed in API endpoint and request parameter.
