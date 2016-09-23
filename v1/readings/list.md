## **GET** /readings

> Get list of `reading`

### **QUERY STRING PARAMETERS**

| Name      | Type    | Values                     | Default | Description             | Required |
| --------- | ------- | -------------------------- | ------- | ----------------------- | -------- |
| type      | string  | article, blog, news, press |    1    | reading type            |     N    |
| page      | integer | integer                    |    1    | current page            |     N    |
| page_size | integer | integer                    |   10    | number of rows per page |     N    |

### **RESPONSE**

``` js
{
  "data": {
    "readings": [
      {
        "id": "reading id",
        "title": "reading title",
        "slug": "reading slug",
        "views": "reading views count",
        "shares": "reading shares count",
        "type": {
            "id": "reading type id",
            "name": "reading type name"
          },
        "isFeatured": "indicate wheter readings is in featured",
        "content": "reading contents",
        "source": "reading source",
        "url": "reading reference url",
        "image": "reading image path",
        "thumbnail": "reading image thumbnail path"
      },
      ...
    ],
    "pagination": {
      "page": "current page",
      "pageSize": "number of entries per page",
      "rowCount": "total entries",
      "pageCount": "total page"
    }
  }
}
```