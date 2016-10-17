## **PUT** /jobs/:id/shares

> Increase `job` shares count

### **URL PARAMETERS**

| Name | Type    | Values  | Default | Description | Required |
| ---- | ------- | ------- | ------- | ----------- | -------- |
| id   | integer | integer |  null   | job id      |     Y    |

### **RESPONSE**

``` js
{
  "data": {
    "shares": "updated job shares count",
  }
}
```