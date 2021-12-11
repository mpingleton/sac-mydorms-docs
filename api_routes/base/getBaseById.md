# Get Base By ID

## GET /api/base/:id

Get information about a specific base given the ID of that base.

## Access Control

Only authenticated users presenting a valid JWT token may access this route.

## Expected Inputs

### Params

- id: An integer corresponding to the ID of the requested base.

### Headers

- Authorization: Bearer ${jwtAccessToken}

### Body

No body expected.

## Output

### 200

A `200 OK` response will be sent with the response body containing a JSON object containing information about the requested base.