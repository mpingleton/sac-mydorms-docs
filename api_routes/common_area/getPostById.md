# Get Post By ID

## GET /api/commonarea/id/:id/

Get a specific common area post given an ID.

## Access Control

Only authenticated users presenting a valid JWT token may access this route.

## Expected Inputs

### Params

- id: An integer corresponding to the ID of the requested post.

### Headers

- Authorization: Bearer ${jwtAccessToken}

### Body

No body expected.

## Output

### 200

A `200 OK` response will be sent with the response body containing a JSON object containing the post information.