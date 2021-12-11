# Login

## POST /api/auth/login

Takes login credentials which will be used to authenticate a user.  Once a 

## Access Control

No access control restrictions exist for this route.

## Expected Inputs

### Params

No params expected.

### Headers

- Content-Type: application/json

### Body

JSON object containing keys:
- "username": A string between 3 and 60 characters long containing the username.
- "password": A string containing the password.

## Output

### 200

A `200 OK` response will be sent upon a successful authentication of a user.  The body of the response will be a JSON object containing the following keys:
- "user": A JSON object containing information about the authenticated user.
- "tokens": A JSON object containing the access and refresh JWT tokens.

### 401

A `401 UNAUTHORIZED` response will be sent under the following conditions:
- The provided login credentials are incorrect. 
- The user account is locked.
- There is a discrepancy between enrollment record data and user roles. 