## Base URL
https://jsonplaceholder.typicode.com

## Get All Users

### Endpoint
GET /users

### Description
Retrieves a list of all users.

### Request
No parameters are required for this request.

### Example Request
GET https://jsonplaceholder.typicode.com/users

### Example Response

[
  {
    "id": 1,
    "name": "Leanne Graham",
    "email": "leanne@example.com"
  }
]
## Get User by ID

### Endpoint
GET /users/{id}

### Description
Retrieves details of a specific user by their ID.

### Parameters

| Name | Type | Description |
|------|------|------------|
| id   | int  | Unique ID of the user |

### Example Request
GET https://jsonplaceholder.typicode.com/users/1

### Example Response

{
  "id": 1,
  "name": "Leanne Graham",
  "email": "leanne@example.com"
}

## Create User

### Endpoint
POST /users

### Description
Creates a new user in the system.

### Request Body

{
  "name": "John Doe",
  "email": "john@example.com"
}

### Example Request
POST https://jsonplaceholder.typicode.com/users

### Example Response

{
  "id": 11,
  "name": "John Doe",
  "email": "john@example.com"
}
### Example Request
POST https://jsonplaceholder.typicode.com/users

### Example Response
{
  "id": 11,
  "name": "John Doe",
  "email": "john@example.com"
}

{
  "name": "John Doe"
}
{
  "id": 11
}
### Headers
Content-Type: application/json

