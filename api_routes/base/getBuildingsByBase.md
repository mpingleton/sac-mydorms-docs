# Get Buildings By Base

## GET /api/base/buildings/:base_id

Get a list of buildings located at a specified base.

## Access Control

Only authenticated users presenting a valid JWT token may access this route.

## Expected Inputs

### Params

- base_id: An integer corresponding to the ID of the requested base.

### Headers

- Authorization: Bearer ${jwtAccessToken}

### Body

No body expected.

## Output

### 200

A `200 OK` response will be sent with the response body containing a JSON array of buildings.