---
sidebar_position: 1
---

# Authentication

API Documentation for authentication purpose

## 📁 Collection: register-merchant

### Method: POST

>```
>{{baseUrl}}/api/auth/register-merchant
>```

### Headers

| Content-Type | Value            |
| ------------ | ---------------- |
| Content-Type | application/json |


### Headers

| Content-Type | Value            |
| ------------ | ---------------- |
| Accept       | application/json |


### Body (**raw**)

```json
{
  "address": "<string>",
  "password": "<string>",
  "phone": "<string>",
  "shopName": "<string>",
  "username": "<string>"
}
```

### Response: 200

```json
{
  "statusCode": "<integer>",
  "message": "<string>",
  "data": {
    "username": "<string>",
    "roles": [
      "<string>",
      "<string>"
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

## 📁 Collection: register-customer


### Method: POST

>```
>{{baseUrl}}/api/auth/register-customer
>```

### Headers

| Content-Type | Value            |
| ------------ | ---------------- |
| Content-Type | application/json |


### Headers

| Content-Type | Value            |
| ------------ | ---------------- |
| Accept       | application/json |


### Body (**raw**)

```json
{
  "address": "<string>",
  "name": "<string>",
  "password": "<string>",
  "phone": "<string>",
  "username": "<string>"
}
```

### Response: 200

```json
{
  "statusCode": "<integer>",
  "message": "<string>",
  "data": {
    "username": "<string>",
    "roles": [
      "<string>",
      "<string>"
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

## 📁 Collection: login


### Method: POST

>```
>{{baseUrl}}/api/auth/login
>```

### Headers

| Content-Type | Value            |
| ------------ | ---------------- |
| Content-Type | application/json |


### Headers

| Content-Type | Value            |
| ------------ | ---------------- |
| Accept       | application/json |


### Body (**raw**)

```json
{
  "password": "<string>",
  "username": "<string>"
}
```

### Response: 200

```json
{
  "statusCode": "<integer>",
  "message": "<string>",
  "data": {
    "id": "<string>",
    "username": "<string>",
    "token": "<string>",
    "roles": [
      "<string>",
      "<string>"
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