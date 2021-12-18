# Get Common Area Post Comment By ID

## GET /api/commonarea/comments/id/:id

Get a single comment given an ID.

## Access Control

Only authenticated users presenting a valid JWT token may access this route.

## Expected Inputs

### Params

- id: An integer corresponding to the ID of the requested comment.

### Headers

- Authorization: Bearer ${jwtAccessToken}

### Body

No body expected.

## Output

### 200

A `200 OK` response with a body containing a JSON object containing the comment.