# REST API with Flask - User Management

## Objective

Build a RESTful API using Flask to manage user data in-memory.

## Features

* GET all users
* GET a user by ID
* POST a new user
* PUT to update a user
* DELETE a user

## Tools & Technologies

* Python
* Flask
* Postman or Curl (for testing)

## Setup Instructions

1. **Clone the Repository**

   ```bash
   git clone <your-repo-url>
   cd <project-directory>
   ```

2. **Install Dependencies**

   ```bash
   pip install flask
   ```

3. **Run the Flask Application**

   ```bash
   python app.py
   ```

   The server will start at `http://127.0.0.1:5000`

## API Endpoints

### GET /users

* **Description:** Fetch all users
* **Response:** `200 OK`

### GET /users/<id>

* **Description:** Fetch user by ID
* **Response:** `200 OK` or `404 Not Found`

### POST /users

* **Description:** Add a new user
* **Body (JSON):** `{ "name": "John", "email": "john@example.com" }`
* **Response:** `201 Created`

### PUT /users/<id>

* **Description:** Update existing user
* **Body (JSON):** `{ "name": "Updated Name", "email": "new@example.com" }`
* **Response:** `200 OK` or `404 Not Found`

### DELETE /users/<id>

* **Description:** Delete user
* **Response:** `200 OK` or `404 Not Found`

## Notes

* This API uses in-memory storage (Python dictionary).
* All changes will be lost when the server restarts.


