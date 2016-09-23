## **GET** /jobs

> Get active `jobs` list

### **QUERY STRING PARAMETERS**

| Name        | Type    | Values                                    | Default | Description             | Required |
| ----------- | ------- | ----------------------------------------- | ------- | ----------------------- | -------- |
| keyword     | string  | string                                    |  null   | keyword to search       |     N    |
| category    | integer | integer                                   |  null   | category id             |     N    |
| subcategory | integer | integer                                   |  null   | subcategory id          |     N    |
| salary_type | integer | integer                                   |  null   | salary type id          |     N    |
| location    | string  | string                                    |  null   | location to search      |     N    |
| workload    | string  | fulltime, parttime, internship, freelance |  null   | job type                |     N    |
| page        | integer | integer                                   |    1    | current page            |     N    |
| page_size   | integer | integer                                   |   10    | number of rows per page |     N    |

### **RESPONSE**

``` js
{
  "data": {
    "jobs": [
      {
        "id": "job id",
        "title": "job title",
        "slug": "job slug",
        "views": "job views count",
        "closedAt": "job closing date",
        "shares": "job shares count",
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
        "intro": "job introduction",
        "attachments": [
          {
            "name": "file name",
            "url": "file url",
            "thumbnail": "file thumbnail url, only exist for image file"
          }
        ],
        "applicants": "number of applicants"
      },
      ...
    ],
    "pagination": {
      "page": "current page",
      "pageSize": "number of entries per page",
      "rowCount": "total entries",
      "pageCount": "total pages count"
    }
  }
}
```