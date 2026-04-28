# Posts API Documentation

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
## Post API Documentation
## Base URL 
https://jsonplaceholder.typicode.com

## End Point
`POST /Posts`

## Description
Create a new post

### Request Body
```Json
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
Field Type| Type| Description|
-----------------------------
id| integer|Unique identifier of the post|
title| string|Title of the post |
body| string|content of the post |
userid|integer| ID of the user creating the post |

