---
sidebar_position: 2
---

# Merchant

API Documentation for admin to organize merchant

## 📁 Collection: Get All Merchant
### Method: GET
>```
>{{baseUrl}}/api/merchants
>```
### Headers

|Content-Type|Value|
|---|---|
|Accept|application/json|


### 🔑 Authentication bearer

|Param|value|Type|
|---|---|---|
|token|`bearerToken`|string|


### Response: 200
```json
{
  "statusCode": "<integer>",
  "message": "<string>",
  "data": [
    {
      "id": "<string>",
      "shopName": "<string>",
      "phone": "<string>",
      "address": "<string>"
    },
    {
      "id": "<string>",
      "shopName": "<string>",
      "phone": "<string>",
      "address": "<string>"
    }
  ],
  "paginationResponse": {
    "totalPages": "<integer>",
    "totalElements": "<long>",
    "currentPage": "<integer>",
    "pageSize": "<integer>",
    "hasNext": "<boolean>",
    "hasPrevious": "<boolean>"
  }
}
```
