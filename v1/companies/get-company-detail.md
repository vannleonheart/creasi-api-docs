## **GET** /companies/:id

> Get `company` basic information

### **URL PARAMETERS**

| Name | Type    | Values  | Default | Description | Required |
| ---- | ------- | ------- | ------- | ----------- | -------- |
| id   | integer | integer |  null   | company id  |     Y    |

### **RESPONSE**

``` js
{
  "status": "response status",
  "code": "response code",
  "data": {
    "id": "company id",
    "name": "company name",
    "address": "company address",
    "phone": "company phone no",
    "logo": "company logo url",
    "homepage": "company website url"
  }
}
```