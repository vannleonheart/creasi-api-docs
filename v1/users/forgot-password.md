## **POST** /recover

> Recover user account using `forgot password` feature

### **REQUEST BODY**

| Name     | Type   | Values  | Default | Description        | Required |
| -------- | ------ | ------- | ------- | ------------------ | -------- |
| email    | string | string  |  null   | user email address |     Y    |

### **RESPONSE**

``` js
{
  "status": "ok",
  "code": 200,
  "data": {}
}
```