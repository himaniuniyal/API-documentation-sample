# GET API Documentation

## Get All Posts

## Base URL
https://jsonplaceholder.typicode.com

### Endpoint
`GET /posts`

### Description
Retrieves a list of all posts.

### Example Request
GET https://jsonplaceholder.typicode.com/posts

### Example Response
```json
{
  "userId": 1,
  "id": 1,
  "title": "sample title",
  "body": "sample content"
}
```
### Response Fields

| Field   | Type   | Description                |
|--------|--------|----------------------------|
| userId | integer | ID of the user who created the post |
| id     | integer | Unique ID of the post      |
| title  | string  | Title of the post          |
| body   | string  | Content of the post        |


---------------------------------------------
# Post API Documentation

## Base URL 
https://jsonplaceholder.typicode.com

## Create Post

### Endpoint
```http
POST /posts
```
### Description
Create a new post

### Request Body
```json
{
  "title": "My Post",
  "body": "This is content",
  "userId": 1
}
```

### Example Request
POST /posts

### Example Response
```json
{
  "id": 101,
  "title": "My Post",
  "body": "This is content",
  "userId": 1
}
```
## Response Field
| Field | Type| Description|
|-----------|-------|-----------|
| id| integer|Unique identifier of the post|
| title| string|Title of the post |
| body| string|content of the post |
| userId|integer| ID of the user creating the post |
------------------------------------------------------

# GET API Documentation

## Base URL 
https://jsonplaceholder.typicode.com/

## GET Post By ID

### Endpoint
```http
GET /posts/{id}
```
- `{id}` = dynamic parameter

### Description
Retrieves a single post by its ID.

### Parameters
|Name | Type |Description|
|---------|-----|-----|
|id | integer| unique ID of the post|

### Example Request
```http
GET /posts/1
```

### Response Example
```json
{
  "userId": 1,
  "id": 1,
  "title": "sample title",
  "body": "sample text"
}
```
### Response Fields
| Field   | Type    | Description                          |
|--------|--------|--------------------------------------|
| userId | integer | ID of the user who created the post  |
| id     | integer | Unique identifier of the post        |
| title  | string  | Title of the post                    |
| body   | string  | Content of the post                  |

----------------------------------------------------------------
# GET API Documentation

## Base URL
https://jsonplaceholder.typicode.com/

### Endpoint
GET /comments

### Description
Retrieve a list of all comments.

### Example Request
```http
GET /comments
```
### Example Response
```json
{ 
    "postId": 1, 
    "id": 1, 
    "name": "sample text", 
    "email": "email", 
    "body": "sample text" 
  }
```
### Response Fields
|Field| Type| Description|
|---|---|----|
| postID | integer | post ID|
|id | integer | unique user id|
|name | string| name|
| email| string | email id|
| body |string | comment|
------------------------------------------------

# Comments API Documentation

## Base URL
https://jsonplaceholder.typicode.com

## Endpoint
### Endpoint
```http
POST /comments
```

## Description
Creates a new comment.

## Example Request
```http
POST /comments
```

## Request Body
```json
{
  "postId": 1,
  "name": "John Doe",
  "email": "john@example.com",
  "body": "This is a comment"
}
```

## Example Response 
```json
{
  "id": 501,
  "postId": 1,
  "name": "John Doe",
  "email": "john@example.com",
  "body": "This is a comment"
}
```
## Response Fields
|Name|Type|Description|
|---|---|---|
|id |integer | unique identification number|
| postId| integer| post ID|
| name | string |name|
|email| string| email|
|body |string |comment|



