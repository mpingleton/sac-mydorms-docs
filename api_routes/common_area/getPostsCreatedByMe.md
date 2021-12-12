# Get All Posts Created By Me

## GET /api/commonarea/createdbyme/

Get all of the common area posts created by the currently authenticated user.

## Access Control

Only authenticated users presenting a valid JWT token may access this route.

## Expected Inputs

### Params

No params expected.

### Headers

- Authorization: Bearer ${jwtAccessToken}

### Body

No body expected.

## Output

### 200

A `200 OK` response will contain JSON array containing all of the common area posts.