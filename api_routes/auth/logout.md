# Logout

## POST /api/auth/logout

Terminates the active session for a user and invalidates all access and refresh tokens.

## Access Control

Only authenticated users presenting a valid JWT token may access this route.

## Expected Inputs

### Params

No params expected.

### Headers

- Content-Type: application/json
- Authorization: Bearer ${jwtAccessToken}

### Body

JSON object containing keys:
- "refreshToken": A string containing the user's JWT refresh token.

## Output

### 204

A `204 NO CONTENT` response with an empty body will be send upon a successful logout.