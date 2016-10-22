## **POST** /me/interviews/:id/respond

> Accepting or rejecting `interview invitation` of `authenticated user`

### **HEADERS**

| Name           | Type   | Values  | Default | Description       | Required |
| -------------- | ------ | ------- | ------- | ----------------- | -------- |
| x-access-token | string | string  |  null   | user access token |     Y    |

### **URL PARAMETERS**

| Name | Type    | Values  | Default | Description  | Required |
| ---- | ------- | ------- | ------- | ------------ | -------- |
| id   | integer | integer |  null   | interview id |     Y    |

### **REQUEST BODY**

| Name              | Type    | Values                 | Default | Description                   | Required |
| ----------------- | ------- | ---------------------- | ------- | ----------------------------- | -------- |
| accept            | integer | 0 = reject, 1 = accept |  null   | Accepting/rejecting interview |     Y    |

### **RESPONSE**

``` js
{
  "status": "ok",
  "code": 200,
  "data": {
    "interview": {
      "id": 197,
      "scheduledAt": "interview schedule timestamp",
      "venue": "the venue",
      "contactName": "contact person name",
      "contactPhone": "contact person phone no",
      "note": "additional note",
      "status": "APPROVE/CANCEL",
    }
  }
}
```