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
https://jsonplaceholder.typicode.com/posts

## End Point
`Get/Posts`

## Description
Create a new data list 

### Example request
```Json
{
  "title": "My Post",
  "body": "This is content",
  "userId": 1
}
```

### Example Response
```json
{
  "id": 101,
  "title": "My Post",
  "body": "This is content",
  "userId": 1
}
```

