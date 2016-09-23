## **POST** /me/tickets

> Create new `help ticket` for `authenticated user`

### **HEADERS**

| Name           | Type   | Values  | Default | Description       | Required |
| -------------- | ------ | ------- | ------- | ----------------- | -------- |
| x-access-token | string | string  |  null   | user access token |     Y    |

### **REQUEST BODY**

| Name    | Type   | Values | Default | Description    | Required |
| ------- | ------ | ------ | ------- | -------------- | -------- |
| subject | string | string |  null   | ticket subject |     Y    |
| message | string | string |  null   | ticket message |     Y    |

### **RESPONSE**

``` js
{
  "data": {
    "subject": "ticket sibject",
    "id": "ticket id",
    "message": "ticket message"
  }
}
```