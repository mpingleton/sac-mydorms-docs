# Get Enrollment For Person

## GET /api/enrollment/personnel/:personnelId

Get the enrollment information 

## Access Control

Only authenticated users presenting a valid JWT token may access this route.

## Expected Inputs

### Params

- personnelId: An integer corresponding to the requested person.

### Headers

- Authorization: Bearer ${jwtAccessToken}

### Body

No body expected.

## Output

### 200

A `200 OK` response will be sent with the response body containing a JSON object with the enrollment data.  This JSON object will also contain a userObject and personnelObject.