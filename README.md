# API Testing Basics with Postman

## Project Overview

This project demonstrates my foundational understanding of API testing using Postman. I created and executed requests using the core HTTP methods: GET, POST, PUT, and DELETE.

I used the free JSONPlaceholder API to practice sending requests, validating responses, and understanding how REST APIs behave.

This project is built from a QA perspective, focusing on verifying endpoint functionality, expected results, and response behavior.

---

## Skills Demonstrated

* Creating and organizing API requests in Postman
* Understanding HTTP methods (GET, POST, PUT, DELETE)
* Working with REST APIs
* Sending JSON request bodies
* Reading and interpreting API responses
* Verifying status codes
* Documenting test scenarios and expected results
* Exporting and managing Postman collections

---

## API Used

JSONPlaceholder (Free test API)
https://jsonplaceholder.typicode.com/

---

## Requests Tested

### 1. GET All Posts

**Endpoint:** `/posts`
**Method:** `GET`

**Purpose:**
Retrieve a list of all posts.

**Expected Result:**

* Status Code: 200 OK
* Response body contains a JSON array of post objects

---

### 2. GET Single Post

**Endpoint:** `/posts/1`
**Method:** `GET`

**Purpose:**
Retrieve a specific post by ID.

**Expected Result:**

* Status Code: 200 OK
* Response body contains a single JSON object with post details

---

### 3. POST Create Post

**Endpoint:** `/posts`
**Method:** `POST`

**Purpose:**
Create a new post.

**Request Body:**

```json
{
  "title": "My API test post",
  "body": "This is a practice POST request.",
  "userId": 1
}
```

**Expected Result:**

* Status Code: 201 Created (or similar success response)
* Response returns the created post data

---

### 4. PUT Update Post

**Endpoint:** `/posts/1`
**Method:** `PUT`

**Purpose:**
Update an existing post.

**Request Body:**

```json
{
  "id": 1,
  "title": "Updated API test post",
  "body": "This post was updated using a PUT request.",
  "userId": 1
}
```

**Expected Result:**

* Status Code: 200 OK
* Response shows updated post data

---

### 5. DELETE Post

**Endpoint:** `/posts/1`
**Method:** `DELETE`

**Purpose:**
Delete a post by ID.

**Expected Result:**

* Status Code: 200 OK (or 204 No Content)
* Response confirms the request was accepted

---

## Status Codes Observed

* GET requests returned 200 OK
* POST request returned a success response (resource created)
* PUT request returned 200 OK
* DELETE request returned a successful response

---

## Project Structure

```
api-testing-basics/
├── README.md
├── collections/
│   └── jsonplaceholder-api-tests.json
└── screenshots/
    ├── collection-overview.png
    ├── get-all-posts.png
    ├── get-single-post.png
    ├── post-create-post.png
    ├── put-update-post.png
    └── delete-post.png
```

---

## Screenshots

### Collection Overview

![Collection Overview](screenshots/collection-overview.png)

### GET All Posts

![GET All Posts](screenshots/get-all-posts.png)

### GET Single Post

![GET Single Post](screenshots/get-single-post.png)

### POST Create Post

![POST Create Post](screenshots/post-create-post.png)

### PUT Update Post

![PUT Update Post](screenshots/put-update-post.png)

### DELETE Post

![DELETE Post](screenshots/delete-post.png)

---

## QA Testing Focus

This project was completed from a QA perspective to:

* Validate API endpoint behavior
* Confirm expected responses and status codes
* Practice CRUD operations through API testing
* Document test scenarios clearly for reproducibility

---

## Key Concepts Practiced

* Endpoints
* HTTP methods
* CRUD operations
* JSON request and response structure
* Status code validation
* API workflow testing

---

## What I Learned

Through this project, I gained hands-on experience working with APIs using Postman. I improved my understanding of how HTTP methods interact with endpoints, how to structure requests, and how to verify responses from a QA perspective.

---

## Author

JonD-33
