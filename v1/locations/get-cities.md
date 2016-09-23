## **GET** /cities

> Get list of `cities`

### **QUERY STRING PARAMETERS**

| Name     | Type    | Values  | Default | Description | Required |
| -------- | ------- | ------- | ------- | ----------- | -------- |
| province | integer | integer |  null   | province id |     Y    |

### **RESPONSE**

``` js
{
  "data": {
    "cities": [
      {
        "id": "city id",
        "name": "city name"
      },
      ...
    ]
  }
}
```