# Get Common Area Posts by Base

## GET /api/commonarea/base/:base_id

Get all of the common area posts located at a given base.

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

A `200 OK` response will contain JSON array containing all of the common area posts.