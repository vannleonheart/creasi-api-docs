## **POST** /authentication

---

`` User authentication ``

### **REQUEST BODY**

| Name     | Type   | Values  | Default | Description        |
| -------- | ------ | ------- | ------- | ------------------ |
| email    | string | string  | null    | user email address |
| password | string | string  | null    | user password      |


### **RESPONSE**
``` json
{
  "data": {
    "token": "access token",
    "lifetime": "access lifetime in seconds",
    "user": {
      "id": "user id",
      "role": {
        "id": "role id",
        "name": "role name"
      }
    }
  }
}
```