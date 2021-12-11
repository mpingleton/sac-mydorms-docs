# Register

## POST /api/auth/register



## Expected Inputs

### Params

No params expected.

### Headers

Authorization: Bearer ${jwtAccessToken}

Content-Type: application/json

### Body

JSON object containing keys:

"username": A string between 3 and 60 characters long containing the username of the new account.

"password": A string containing the password to assign to the new account.

"code": A string containing the registration code needed to create the account.

## Output

### 201

A `201 CREATED` response is sent upon successful creation of the user account.  It will contain an empty body.

### 400

A `400 BAD REQUEST` response is sent when there is no pending enrollment matching the provided registration code.  The body will contain a plain text `The registration code provided is invalid.`.

