## **GET** /jobs/:id

> Get `job` detail

### **URL PARAMETERS**

| Name | Type    | Values  | Default | Description | Required |
| ---- | ------- | ------- | ------- | ----------- | -------- |
| id   | integer | integer |  null   | job id      |     Y    |

### **RESPONSE**

``` js
{
  "data": {
    "id": "job id",
    "title": "job title",
    "slug": "job slug",
    "views": "job views count",
    "shares": "job shares count",
    "closedAt": "job closing date",
    "status": "job status (DRAFT, IN MODERATION, OPEN, INTERVIEW, CLOSED, UNSUCCESSFUL)",
    "company": {
      "id": "company id",
      "name": "company name"
    },
    "category": {
      "id": "category id",
      "name": "category name"
    },
    "subcategory": {
      "id": "subcategory id",
      "name": "subcategory name"
    },
    "province": {
      "id": "province id",
      "name": "province name"
    },
    "city": {
      "id": "city id",
      "name": "city name"
    },
    "salary": {
      "id": "salary id",
      "label": "salary label text"  
    },
    "type": [ "array of job type (freelance, fulltime, parrtime, internship)" ],
    "description": "job description",
    "benefits": "job benefits",
    "requirements": "job requirements",
    "intro": "job introduction,
    "applicants": "number of applicants",
    "attachments": [
      {
        "name": "file name",
        "url": "file url",
        "thumbnail": "file thumbnail url, only exist for image file"
      }
    ],
    "url": "url job for sharing",
    "applied": "indicate current user has been applied or not (true, false)"
  }
}
```