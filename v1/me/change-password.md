## **PUT** /me/password

> Change `authenticated user` password

### **HEADERS**

| Name           | Type   | Values  | Default | Description       | Required |
| -------------- | ------ | ------- | ------- | ----------------- | -------- |
| x-access-token | string | string  |  null   | user access token |     Y    |

### **REQUEST BODY**

| Name                      | Type    | Values | Default | Description               | Required |
| ------------------------- | ------  | ------ | ------- | ------------------------- | -------- |
| password                  | string  | string |  null   | user current password     |     Y    |
| new_password              | string  | string |  null   | user new password         |     Y    |
| new_password_confirmation | string  | string |  null   | new password confirmation |     Y    |

### **RESPONSE**

``` js
{
  "data": {
    
  }
}
```