## **DELETE** /me

> Deactivate `authenticated user` current account

### **HEADERS**

| Name           | Type   | Values  | Default | Description       | Required |
| -------------- | ------ | ------- | ------- | ----------------- | -------- |
| x-access-token | string | string  |  null   | user access token |     Y    |

### **REQUEST BODY**

| Name     | Type   | Values | Default | Description          | Required |
| -------- | ------ | ------ | ------- | -------------------- | -------- |
| reason   | string | string |  null   | deactivation reason  |     Y    |
| message  | string | string |  null   | deactivation message |     Y    |
| password | string | string |  null   | user password        |     Y    |

### **RESPONSE**

``` js
{
  "data": {
    
  }
}
```