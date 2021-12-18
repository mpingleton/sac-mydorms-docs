# Get My Enrollment

## GET /api/enrollment/my

Get the enrollment information for the currently authenticated user.

## Access Control

Only authenticated users presenting a valid JWT token may access this route.

## Expected Inputs

### Params

No params expected.

### Headers

- Authorization: Bearer ${jwtAccessToken}

### Body

No body expected.

## Output

### 200

A `200 OK` response will be sent with the response body containing a JSON object with the enrollment data.  This JSON object will also contain a userObject and personnelObject.