## **PUT** /me/email

> Change `authenticated user` email

### **HEADERS**

| Name           | Type   | Values  | Default | Description       | Required |
| -------------- | ------ | ------- | ------- | ----------------- | -------- |
| x-access-token | string | string  |  null   | user access token |     Y    |

### **REQUEST BODY**

| Name               | Type    | Values | Default | Description            | Required |
| ------------------ | ------  | ------ | ------- | ---------------------- | -------- |
| email              | string  | string |  null   | user new email address |     Y    |
| email_confirmation | string  | string |  null   | new email confirmation |     Y    |
| password           | string  | string |  null   | user password          |     Y    |

### **RESPONSE**

``` js
{
  "data": {
    "id": "email id",
    "email": "new email address"
  }
}
```