# Get All Posts Created By

## GET /api/commonarea/postedby/:personnel_id

Get all of the common area posts created by a given person.

## Access Control

Only authenticated users presenting a valid JWT token may access this route.

## Expected Inputs

### Params

- personnel_id: An integer corresponding to the ID of the requested person.

### Headers

- Authorization: Bearer ${jwtAccessToken}

### Body

No body expected.

## Output

### 200

A `200 OK` response will contain JSON array containing all of the common area posts.