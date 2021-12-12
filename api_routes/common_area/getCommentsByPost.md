# Get Common Area Post Comments

## GET /api/commonarea/comments/post/:id

Get all of the comments that are associated with a given post.

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

A `200 OK` response with a body containing a JSON array with all of the comments.

