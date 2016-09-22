## **POST** /users/creative-talents

> Create new user account as `creative talent`

### **REQUEST BODY**

| Name     | Type   | Values  | Default | Description        | Required |
| -------- | ------ | ------- | ------- | ------------------ | -------- |
| name     | string | string  | null    | user full name     | Y        |
| phone    | string | string  | null    | user phone no      | Y        |
| email    | string | string  | null    | user email address | Y        |
| password | string | string  | null    | user password      | Y        |
| cv       | file   | file    | null    | user cv file       | N        |

### **RESPONSE**
``` js
{
  "data": {
    "user": {
      "name": "user name",
      "phone": "user phone no",
      "id": "user id"
    },
    "email": {
      "email": "user email address",
      "id": "user email id"
    }
  }
}
```

