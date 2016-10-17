## **GET** /me/announcements

> Get `authenticated user` notifications

### **HEADERS**

| Name           | Type   | Values  | Default | Description       | Required |
| -------------- | ------ | ------- | ------- | ----------------- | -------- |
| x-access-token | string | string  |  null   | user access token |     Y    |

### **QUERY STRING PARAMETERS**

| Name      | Type    | Values  | Default | Description             | Required |
| --------- | ------- | ------- | ------- | ----------------------- | -------- |
| page      | integer | integer |    1    | current page            |     N    |
| page_size | integer | integer |   10    | number of rows per page |     N    |

### **RESPONSE**

``` js
{
  "data": [
    {
      "id": "announcement id",
      "flag": "notification flag (0 = new, 1 = unread, 2 = read)",
      "message": {
        "subject": "message subject",
        "image": "message image url",
        "content": "message body"
      }
    },
    ...
  ]
}
```