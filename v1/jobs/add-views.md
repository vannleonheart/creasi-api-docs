## **POST** /jobs/:id/views

> Increase `job` views count

### **URL PARAMETERS**

| Name | Type    | Values  | Default | Description | Required |
| ---- | ------- | ------- | ------- | ----------- | -------- |
| id   | integer | integer |  null   | job id      |     Y    |

### **RESPONSE**

``` js
{
  "data": {
    "views": "updated job views count",
  }
}
```