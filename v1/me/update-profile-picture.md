## **PUT** /me/avatar

> Update `authenticated user` profile picture

### **HEADERS**

| Name           | Type   | Values  | Default | Description       | Required |
| -------------- | ------ | ------- | ------- | ----------------- | -------- |
| x-access-token | string | string  |  null   | user access token |     Y    |

### **REQUEST BODY**

| Name   | Type    | Values  | Default | Description                 | Required |
| ------ | ------  | ------- | ------- | --------------------------- | -------- |
| avatar | file    | file    |  null   | user profile picture file   |     Y    |
| width  | integer | integer |  null   | resize image to this width  |     Y    |
| height | integer | integer |  null   | resize image to this height |     Y    |
| x      | integer | integer |  null   | crop image from x position  |     Y    |
| y      | integer | integer |  null   | crop image from y position  |     Y    |
| rotate | integer | integer |  null   | rotate image                |     Y    |
| scaleX | integer | integer |  null   | scale image width           |     Y    |
| scaleY | integer | integer |  null   | scale image height          |     Y    |

### **RESPONSE**

``` js
{
  "data": {
    "url": "image url"
  }
}
```