---
sidebar_position: 3
---

# Customer

API Documentation for admin to organize customer

## End-point: Get All Customer
### Method: GET
>```
>{{baseUrl}}/api/customers
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
      "name": "<string>",
      "address": "<string>",
      "phone": "<string>",
      "pointTransaction": "<integer>"
    },
    {
      "id": "<string>",
      "name": "<string>",
      "address": "<string>",
      "phone": "<string>",
      "pointTransaction": "<integer>"
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
