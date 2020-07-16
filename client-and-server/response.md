# Guide on response from server

## Response

In order to stay in sync we have to response with data with specific **response code**.
From server you'll send response JSON in following structure:

```javascript
{
  success: true/false,
  data: [...],
  message: 'Either empty or some message depending upon requirement'
}
```

## Status codes

It is very important to sent a status code in every request. Here is the complete list of status codes that you'll send

| **Code** | **Short**          | **Long**                                 |
| -------- | ------------------ | ---------------------------------------- |
| 200      | OK                 | Operation is successful                  |
| 400      | Bad Request        | Required parameters not provided         |
| 401      | Unauthorised       | User is not have valid authentication    |
| 402      | Payment expired    | Subscription has expired                 |
| 403      | Forbidden          | Data is valid but user have no access    |
| 404      | `Never use`        | I repeat `Never use`                     |
| 405      | Method not allowed | User is locked by admin                  |
| 500      | Server error       | Something went wrong with server         |
| 503      | Database error     | Something went wrong while with database |
