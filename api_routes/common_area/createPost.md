# Create Post

## PUT /api/commonarea/

Submits a post to the common area.

## Access Control

Only authenticated users presenting a valid JWT token may access this route.

## Expected Inputs

### Params

No params 

### Headers

- Content-Type: application/json
- Authorization: Bearer ${jwtAccessToken}

### Body

A JSON object containing the following keys:
- "text": A string which may be up to 1000 characters in length that contains the text of the post.

## Output

### 200

A `200 OK` response with an empty response body is sent upon a successful posting.