# Create a Building

## PUT /api/base/buildings/

Create a building and insert it into the database.

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
- "base_id": An integer containing the ID of the base where this building is located.
- "building_number": A string containing the number of the building.
- "building_name": A string containing the name of the building.
- "address": A string containing the address of the building.

## Output

### 201

A `201 CREATED` response with an empty body will be sent upon the successful creation of the building.