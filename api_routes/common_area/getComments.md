# Get Common Area Post Comments

## GET /api/commonarea/comments

Get all of the common area posts that are stored in the database.

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

A `200 OK` response with a body containing a JSON array with all of the comments.

