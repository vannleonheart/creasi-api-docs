## **GET** /subcategories

> Get list of job `subcategory`

### **QUERY STRING PARAMETERS**

| Name     | Type    | Values  | Default | Description | Required |
| -------- | ------- | ------- | ------- | ----------- | -------- |
| category | integer | integer |  null   | category id |     Y    |

### **RESPONSE**

``` js
{
  "data": {
    "subcategories": [
      {
        "id": "subcategory id",
        "name": "subcategory name"
      },
      ...
    ]
  }
}
```