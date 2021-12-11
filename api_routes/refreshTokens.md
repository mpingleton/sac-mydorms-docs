# Refresh Tokens

## POST /api/auth/refresh-tokens

Refreshes an authenticated user's JWT token.

## Access Control

Only authenticated users presenting a valid JWT token may access this route.

## Expected Inputs

### Params

No params expected.

### Headers

- Content-Type: application/json

### Body

JSON object containing keys:
- "refreshToken": A string containing the user's JWT refresh token.

## Output

### 200

A `200 OK` response will be sent upon a successful refresh of a user's JWT access token.  The body of the response will be a JSON object containing the following keys:
- "user": A JSON object containing information about the authenticated user.
- "tokens": A JSON object containing the access and refresh JWT tokens.


