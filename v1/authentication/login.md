## **POST** /authentication

> Generate `access token` for user as identity for future request (request as `authenticated user`)

### **REQUEST BODY**

| Name     | Type   | Values  | Default | Description        | Required |
| -------- | ------ | ------- | ------- | ------------------ | -------- |
| email    | string | string  | null    | user email address | Y        |
| password | string | string  | null    | user password      | Y        |


### **RESPONSE**
``` js
{
  "data": {
    "token": "access token",
    "lifetime": "access lifetime in seconds",
    "user": {
      "id": "user id",
      "role": {
        "id": "role id",
        "name": "role name"
      }
    }
  }
}
```