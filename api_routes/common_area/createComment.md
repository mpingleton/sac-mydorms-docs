# Create Comment

## PUT /api/commonarea/comments

Post a comment on a given post.

## Access Control

Only authenticated users presenting a valid JWT token may access this route.

## Expected Inputs

### Params

No params expected.

### Headers

- Content-Type: application/json
- Authorization: Bearer ${jwtAccessToken}

### Body

A JSON object containing the following keys:
- "post_id": An integer corresponding to the ID of the post that this comment should be associated with.
- "text": A string up to 1000 characters in length that contains the contents of the comment.

## Output

### 200

A `200 OK` response with an empty body will be returned upon posting the comment.

