## **PUT** /me

> Update `authenticated user` basic information

### **HEADERS**

| Name           | Type   | Values  | Default | Description       | Required |
| -------------- | ------ | ------- | ------- | ----------------- | -------- |
| x-access-token | string | string  |  null   | user access token |     Y    |

### **REQUEST BODY**

| Name              | Type    | Values       | Default | Description               | Required |
| ----------------- | ------- | ------------ | ------- | ------------------------- | -------- |
| name              | string  | string       |  null   | user full name            |     Y    |
| gender            | string  | male, female |  null   | user gender               |     Y    |
| phone             | string  | string       |  null   | user phone no             |     Y    |
| province          | integer | integer      |  null   | province id               |     N    |
| city              | integer | integer      |  null   | city id                   |     N    |
| birth_date        | integer | 1 .. 31      |  null   | user birth date           |     Y    |
| birth_month       | integer | 1 .. 12      |  null   | user birth month          |     Y    |
| birth_year        | integer | integer      |  null   | user birth year           |     Y    |
| cv                | file    | file         |  null   | user cv file              |     Y    |
| facebookUsername  | string  | string       |  null   | user facebook username    |     Y    |
| twitterScreenName | string  | string       |  null   | user twitter sceen name   |     Y    |
| instagramUsername | string  | string       |  null   | user instagram sceen name |     Y    |
| youtubeUsername   | string  | string       |  null   | user youtube sceen name   |     Y    |
| homepage          | string  | string       |  null   | user homepage url         |     Y    |

### **RESPONSE**

``` js
{
  "status": "response status",
  "code": "response code",
  "data": {
    "id": "user id",
    "name": "user name",
    "gender": "user gender",
    "birthdate": "birthdate",
    "phone": "user contact number",
    "role": {
      "id": "role id",
      "name": "role name"
    },
    "province": {
      "id": "province id",
      "name": "province name"
    },
    "city": {
      "id": "city id",
      "name": "city name"
    },
    "type": {
      "id": "user type id",
      "name": "user type name"
    },
    "facebookUsername": "user facebook username",
    "twitterScreenName": "user twitter username",
    "instagramUsername": "user instagram username",
    "youtubeUsername": "user youtube username",
    "homepage": "user homepage url"
  }
}
```
