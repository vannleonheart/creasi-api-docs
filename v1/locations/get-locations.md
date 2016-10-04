## **GET** /cities

> Get list of `locations`

### **QUERY STRING PARAMETERS**

| Name   | Type   | Values | Default | Description        | Required |
| ------ | ------ | ------ | ------- | ------------------ | -------- |
| search | string | string |  null   | province/city name |     N    |

### **RESPONSE**

``` js
{
  "status": "ok",
  "code": 200,
  "data": {
    "locations": [
      {
        "name": "DKI Jakarta"
      },
      {
        "name": "Jakarta Barat"
      },
      {
        "name": "Jakarta Pusat"
      },
      {
        "name": "Jakarta Selatan"
      },
      {
        "name": "Jakarta Timur"
      },
      {
        "name": "Jakarta Utara"
      }
    ]
  }
}
```