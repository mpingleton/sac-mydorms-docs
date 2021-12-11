# Me

## GET /api/auth/me

Returns information about an authenticated user based on the JWT token provided.

## Access Control

Only authenticated users presenting a valid JWT token may access this route.

## Expected Inputs

### Params

No params expected.

### Headers

- Content-Type: application/json
- Authorization: Bearer ${jwtAccessToken}

### Body

No body expected.

## Output

### 200

The body of the response will be a JSON object containing the following keys:
- "user": A JSON object containing information about the authenticated user.
