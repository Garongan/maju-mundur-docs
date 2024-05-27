---
sidebar_position: 6
---

# Claim Reward

API Documentation for claim reward

## End-point: Claim Reward
### Method: POST
>```
>{{baseUrl}}/api/claim-rewards
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
  "customerId": "<string>",
  "rewardId": "<string>"
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
    "claimDate": "<string>",
    "customerId": "<string>",
    "rewardId": "<string>"
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