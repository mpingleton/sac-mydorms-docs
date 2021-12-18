# Get All Enrollments

## GET /api/enrollment/

Get all of the user and personnel record enrollments in the database.

## Access Control

Only authenticated users presenting a valid JWT token may access this route.

Only dorm managers may access this route.

This route may be accessed by residents or dorm managers.

Only residents may access this route.

## Expected Inputs

### Params

No params expected.

### Headers

- Authorization: Bearer ${jwtAccessToken}

### Body

No body expected.

## Output

### 200

A `200 OK` response with a body containing a JSON object containing an array of enrollments.

