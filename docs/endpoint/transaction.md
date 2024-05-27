---
sidebar_position: 7
---

# Transaction

API Documentation for transaction

## End-point: Get Merchant History Transaction
### Method: GET
>```
>{{baseUrl}}/api/transactions/history
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
      "transactionDate": "<string>",
      "pointEarned": "<integer>",
      "customerId": "<string>",
      "details": [
        {
          "id": "<string>",
          "quantity": "<integer>",
          "price": "<long>",
          "productId": "<string>"
        },
        {
          "id": "<string>",
          "quantity": "<integer>",
          "price": "<long>",
          "productId": "<string>"
        }
      ]
    },
    {
      "id": "<string>",
      "transactionDate": "<string>",
      "pointEarned": "<integer>",
      "customerId": "<string>",
      "details": [
        {
          "id": "<string>",
          "quantity": "<integer>",
          "price": "<long>",
          "productId": "<string>"
        },
        {
          "id": "<string>",
          "quantity": "<integer>",
          "price": "<long>",
          "productId": "<string>"
        }
      ]
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

## End-point: Get all transactions
### Method: GET
>```
>{{baseUrl}}/api/transactions
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
      "transactionDate": "<string>",
      "pointEarned": "<integer>",
      "customerId": "<string>",
      "details": [
        {
          "id": "<string>",
          "quantity": "<integer>",
          "price": "<long>",
          "productId": "<string>"
        },
        {
          "id": "<string>",
          "quantity": "<integer>",
          "price": "<long>",
          "productId": "<string>"
        }
      ]
    },
    {
      "id": "<string>",
      "transactionDate": "<string>",
      "pointEarned": "<integer>",
      "customerId": "<string>",
      "details": [
        {
          "id": "<string>",
          "quantity": "<integer>",
          "price": "<long>",
          "productId": "<string>"
        },
        {
          "id": "<string>",
          "quantity": "<integer>",
          "price": "<long>",
          "productId": "<string>"
        }
      ]
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

## End-point: Create new transaction
### Method: POST
>```
>{{baseUrl}}/api/transactions?customerId=<string>&details=[object Object],[object Object]
>```
### Headers

|Content-Type|Value|
|---|---|
|Accept|application/json|


### Query Params

|Param|value|
|---|---|
|customerId|string|
|details|[object Object],[object Object]|


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
    "transactionDate": "<string>",
    "pointEarned": "<integer>",
    "customerId": "<string>",
    "details": [
      {
        "id": "<string>",
        "quantity": "<integer>",
        "price": "<long>",
        "productId": "<string>"
      },
      {
        "id": "<string>",
        "quantity": "<integer>",
        "price": "<long>",
        "productId": "<string>"
      }
    ]
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