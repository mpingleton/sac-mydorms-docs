# Create an Enrollment

## PUT /api/enrollment/

Create an enrollment for a user.

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

- userId: An integer corresponding to the user record.
- personnelId: An integer corresponding to the personnel record.

## Output

### 200

A `200 OK` with an empty body will be sent upon the creation of an enrollment.