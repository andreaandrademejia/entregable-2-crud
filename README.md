# api-crud-2

User Management CRUD API
This API allows you to perform CRUD (Create, Read, Update, Delete) operations on users in the system. It is built with Node.js, Express, and Sequelize, using PostgreSQL as the database.
API Structure
The API follows the RESTful principle and offers the following endpoints:
GET /users: Gets all users.
POST /users: Creates a new user.
GET /users/:id: Gets a specific user by its ID.
PUT /users/:id: Updates a specific user by its ID.
DELETE /users/:id: Deletes a specific user by its ID.

Authentication
You can require authentication using JWT tokens in the Authorization header.
Error Handling
HTTP status codes returned include:
200 OK: Successful request.
201 Created: Resource created.
204 No Content: Operation successful, no content.
400 Bad Request: Invalid request.
404 Not Found: Resource does not exist.
500 Internal Server Error: Server error.

Usage Example
To create a user, send a POST request to /users with the following body:

```json
{
	"firstName": "John",
	"lastName": "Doe",
	"email": "john.doe@example.com",
	"password": "password123",
	"birthday": "1990-01-01"
}
```
