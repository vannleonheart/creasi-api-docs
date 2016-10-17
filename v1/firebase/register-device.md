## **POST** /devices

> Registering `device id` on firebase

### **HEADERS**

| Name           | Type   | Values  | Default | Description       | Required |
| -------------- | ------ | ------- | ------- | ----------------- | -------- |
| x-access-token | string | string  |  null   | user access token |     Y    |

### **REQUEST BODY**

| Name     | Type    | Values | Default | Description | Required |
| -------- | ------- | ------ | ------- | ----------- | -------- |
| device   | string  | string |  null   | device id   |     Y    |
| firebase | string  | string |  null   | firebase id |     Y    |

### **RESPONSE**

``` js
{
  "status": "ok",
  "code": 200,
  "data": {
    "id": 1,
    "userId": 1820,
    "deviceId": "device id",
    "firebaseId": "firebase id",
    "enable": 1,
  }
}
```