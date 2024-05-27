---
sidebar_position: 5
---

# Reward

API Documentation for reward given after transaction made by customer

## End-point: Get reward by id
### Method: GET
>```
>{{baseUrl}}/api/rewards/:id
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
  "data": {
    "id": "<string>",
    "name": "<string>",
    "pointRequired": "<integer>",
    "stock": "<integer>"
  },
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

## End-point: Get all rewards
### Method: GET
>```
>{{baseUrl}}/api/rewards
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
      "pointRequired": "<integer>",
      "stock": "<integer>"
    },
    {
      "id": "<string>",
      "name": "<string>",
      "pointRequired": "<integer>",
      "stock": "<integer>"
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

## End-point: Update reward
### Method: PUT
>```
>{{baseUrl}}/api/rewards?id=<string>&name=<string>&pointRequired=<integer>&stock=<integer>
>```
### Headers

|Content-Type|Value|
|---|---|
|Accept|application/json|


### Query Params

|Param|value|
|---|---|
|id|string|
|name|string|
|pointRequired|integer|
|stock|integer|


### 🔑 Authentication bearer

|Param|value|Type|
|---|---|---|
|token|`bearerToken`|string|


### Response: 200
```json
{
  "statusCode": "<integer>",
  "message": "<string>",
  "data": {
    "id": "<string>",
    "name": "<string>",
    "pointRequired": "<integer>",
    "stock": "<integer>"
  },
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

## End-point: Create new reward
### Method: POST
>```
>{{baseUrl}}/api/rewards
>```
### Headers

|Content-Type|Value|
|---|---|
|Content-Type|application/json|


### Headers

|Content-Type|Value|
|---|---|
|Accept|application/json|


### Body (**raw**)

```json
{
  "name": "<string>",
  "pointRequired": "<integer>",
  "stock": "<integer>"
}
```

### 🔑 Authentication bearer

|Param|value|Type|
|---|---|---|
|token|`bearerToken`|string|


### Response: 200
```json
{
  "statusCode": "<integer>",
  "message": "<string>",
  "data": {
    "id": "<string>",
    "name": "<string>",
    "pointRequired": "<integer>",
    "stock": "<integer>"
  },
  "paginationResponse": {
    "totalPages": "<integer>",
    "totalElements": "<long>",
    "currentPage": "<integer>",
    "pageSize": "<integer>",
    "hasNext": "<boolean>",
    "hasPrevious": "<boolean>"
  }
}
