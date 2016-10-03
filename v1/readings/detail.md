## **GET** /readings/:id

> Get `reading` detail

### **URL PARAMETERS**

| Name | Type    | Values  | Default | Description | Required |
| ---- | ------- | ------- | ------- | ----------- | -------- |
| id   | integer | integer |  null   | reading id  |     Y    |

### **RESPONSE**

``` js
{
  "data": {
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
    "source_url": "reading reference url",
    "image": "reading image path",
    "thumbnail": "reading image thumbnail path",
    "url": "reading url for sharing"
  }
}
```