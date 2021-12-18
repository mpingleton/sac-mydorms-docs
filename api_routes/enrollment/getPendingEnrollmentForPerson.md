# Description

## GET /api/enrollment/pending/:personnelId

Get the pending enrollment that exists for the given person.

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

A `200 OK` response with a body containing a JSON object with the pending enrollment information.