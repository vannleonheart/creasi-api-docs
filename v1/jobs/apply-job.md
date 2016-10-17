## **POST** /jobs/:id/applicants

> Apply for specified `job`

### **HEADERS**

| Name           | Type   | Values  | Default | Description       | Required |
| -------------- | ------ | ------- | ------- | ----------------- | -------- |
| x-access-token | string | string  |  null   | user access token |     Y    |

### **URL PARAMETERS**

| Name | Type    | Values  | Default | Description | Required |
| ---- | ------- | ------- | ------- | ----------- | -------- |
| id   | integer | integer |  null   | job id      |     Y    |

### **RESPONSE**

``` js
{
  "data": {
    
  }
}
```