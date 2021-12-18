# Enroll Current User Using Code

## POST /api/enrollment/enrollcurrentuser/using/code

Create an enrollment for the currently enrolled user based on a provided enrollment code.

## Access Control

Only authenticated users presenting a valid JWT token may access this route.

## Expected Inputs

### Params

No params expected.

### Headers

- Authorization: Bearer ${jwtAccessToken}
- Content-Type: application/json

### Body

A JSON object containing the following keys:

- registrationCode: A string containing the enrollment code.

## Output

### 200

A `200 OK` response will sent upon creating the enrollment.