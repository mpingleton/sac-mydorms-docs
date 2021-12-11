# Create a Base

## PUT /api/base/

Create a base and insert it into the database.

## Access Control

Only authenticated users presenting a valid JWT token may access this route.

## Expected Inputs

### Params

No params expected.

### Headers

- Content-Type: application/json
- Authorization: Bearer ${jwtAccessToken}

### Body

A JSON object containing the following keys:
- "name": A string containing the name of the base.

## Output

### 201

A `201 CREATED` response with an empty body will be sent upon the successful creation of the base.