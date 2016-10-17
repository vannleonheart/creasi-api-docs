## **GET** /me/applications

> Get `authenticated user` job applications

### **HEADERS**

| Name           | Type   | Values  | Default | Description       | Required |
| -------------- | ------ | ------- | ------- | ----------------- | -------- |
| x-access-token | string | string  |  null   | user access token |     Y    |

### **QUERY STRING PARAMETERS**

| Name      | Type    | Values    | Default | Description             | Required |
| --------- | ------- | --------- | ------- | ----------------------- | -------- |
| page      | integer | integer   |    1    | current page            |     N    |
| page_size | integer | integer   |   10    | number of rows per page |     N    |
| order     | string  | asc, desc |  desc   | ordering                |     N    |

### **RESPONSE**

``` js
{
  "data": {
    "jobs": [
      {
        "id": "job application id",
        "status": "job application status (APPLIED, INTERVIEW, HIRED)",
        "job": {
          "id": "job id",
          "title": "job title",
          "slug": "job slug",
          "status": "job status (DRAFT, PENDING, IN MODERATION, OPEN, INTERVIEW, CLOSED, UNSUCCESSFULL)",
          "publish": "job publish status (Y, N)",
          "upgradable": "indicate job is upgradable (Y, N)",
          "views": "job views count",
          "likes": "job likes count",
          "shares": "job share count",
          "closedAt": "job closing date",
          "createdAt": "job created date",
          "province": {
            "id": "province id",
            "name": "province name"
          },
          "city": {
            "id": "city id",
            "name": "city name"
          },
          "company": {
            "id": "company id",
            "type": "company type (corporate, independent)",
            "name": "company name",
            "brand": "company brand",
            "email": "company email",
            "address": "company address",
            "phone": "company phone no",
            "province": {
                "id": "province id",
                "name": "province name"
            },
            "city": {
              "id": "city id",
              "name": "city name"
            },
            "logo": "logo url",
            "homepage": "company homepage"
          },
          "type": [ "array of job type (fulltime, parttime, freelance, internship)" ],
          "applicants": "number of applicants" 
        }
      },
      ...
    ]
  }
}
```