---
sidebar_position: 4
---

# Product

API Documentation for product

## 📁 Collection: Get product by id
### Method: GET
>```
>{{baseUrl}}/api/products/:id
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
    "price": "<long>",
    "stock": "<integer>",
    "merchant": {
      "id": "<string>",
      "shopName": "<string>",
      "phone": "<string>",
      "address": "<string>"
    }
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

## 📁 Collection: Delete product
### Method: DELETE
>```
>{{baseUrl}}/api/products/:id?userAccountId=<string>
>```
### Headers

|Content-Type|Value|
|---|---|
|Accept|application/json|


### Query Params

|Param|value|
|---|---|
|userAccountId|string|


### 🔑 Authentication bearer

|Param|value|Type|
|---|---|---|
|token|`bearerToken`|string|


### Response: 200
```json
{
  "statusCode": "<integer>",
  "message": "<string>",
  "data": "<string>",
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

## 📁 Collection: Get all products
### Method: GET
>```
>{{baseUrl}}/api/products?direction=asc&orderBy=name&currentPage=1&pageSize=10
>```
### Headers

|Content-Type|Value|
|---|---|
|Accept|application/json|


### Query Params

|Param|value|
|---|---|
|direction|asc|
|orderBy|name|
|currentPage|1|
|pageSize|10|


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
      "price": "<long>",
      "stock": "<integer>",
      "merchant": {
        "id": "<string>",
        "shopName": "<string>",
        "phone": "<string>",
        "address": "<string>"
      }
    },
    {
      "id": "<string>",
      "name": "<string>",
      "price": "<long>",
      "stock": "<integer>",
      "merchant": {
        "id": "<string>",
        "shopName": "<string>",
        "phone": "<string>",
        "address": "<string>"
      }
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

## 📁 Collection: Update product
### Method: PUT
>```
>{{baseUrl}}/api/products
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
  "id": "<string>",
  "name": "<string>",
  "userAccountId": "<string>",
  "price": "<long>",
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
    "price": "<long>",
    "stock": "<integer>",
    "merchant": {
      "id": "<string>",
      "shopName": "<string>",
      "phone": "<string>",
      "address": "<string>"
    }
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

## 📁 Collection: Create new product
### Method: POST
>```
>{{baseUrl}}/api/products
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
  "userAccountId": "<string>",
  "price": "<long>",
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
    "price": "<long>",
    "stock": "<integer>",
    "merchant": {
      "id": "<string>",
      "shopName": "<string>",
      "phone": "<string>",
      "address": "<string>"
    }
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
