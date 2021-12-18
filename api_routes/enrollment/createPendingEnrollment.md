# Create a Pending Enrollment

## PUT /api/enrollment/pending

Create a pending enrollment and registration code for a person.

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
- personnelId: An integer corresponding to the requested person.

## Output

### 201

A `201 CREATED` response will be sent with the body being a JSON object containing the personnelId and registrationCode.