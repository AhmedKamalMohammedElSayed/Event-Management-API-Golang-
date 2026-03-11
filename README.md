# Event Management API (Golang)

A RESTful **Event Management Backend API** built with **Go (Golang)**.  
This project demonstrates how to build a complete backend including **CRUD operations, authentication with JWT, password hashing, middleware, and authorization**.

The project is structured step-by-step to show the development process from creating the server to implementing authentication and event registration.

---

## Features

- Create and manage events
- Retrieve all events from database
- Get a single event by ID
- Update events
- Delete events
- User registration
- Password hashing for security
- JWT authentication
- Token verification middleware
- Authorization for protected routes
- Event registration and cancellation

---

## Project Structure

```
01-starting-project
02-first-route-request-handler
03-testing-requests-fixing-post-request
04-getting-events-from-database
05-get-single-event
06-refactoring-code
07-updating-events
08-deleting-events
09-adding-user-signup
10-hashing-passwords
11-generating-jwt
12-adding-token-verification
13-enhancing-auth-middleware
14-adding-authorization
15-testing-fixing-register-route
16-cancelling-registrations
```

Each folder represents a **development step** in building the backend system.

---

## Technologies Used

- Go (Golang)
- REST API
- JWT Authentication
- bcrypt (Password Hashing)
- SQL Database
- HTTP Middleware

---

## API Endpoints

### Events

| Method | Endpoint      | Description      |
| ------ | ------------- | ---------------- |
| GET    | `/events`     | Get all events   |
| GET    | `/events/:id` | Get single event |
| POST   | `/events`     | Create event     |
| PUT    | `/events/:id` | Update event     |
| DELETE | `/events/:id` | Delete event     |

---

### Authentication

| Method | Endpoint  | Description                |
| ------ | --------- | -------------------------- |
| POST   | `/signup` | Register new user          |
| POST   | `/login`  | Login user and receive JWT |

---

### Event Registration

| Method | Endpoint               | Description         |
| ------ | ---------------------- | ------------------- |
| POST   | `/events/:id/register` | Register for event  |
| DELETE | `/events/:id/register` | Cancel registration |

---

## Installation

Clone the repository

```bash
git clone https://github.com/yourusername/event-management-go.git
```

Navigate to the project folder

```bash
cd event-management-go
```

Install dependencies

```bash
go mod tidy
```

Run the server

```bash
go run main.go
```

---

## Authentication

The API uses **JWT tokens** for authentication.

After logging in, include the token in requests:

```
Authorization: Bearer <your_token>
```

---

## Learning Goals

This project demonstrates:

- Building REST APIs in Go
- Structuring backend applications
- Implementing authentication and authorization
- Working with databases
- Writing middleware
- Secure password handling

---

## Future Improvements

- Docker support
- Unit testing
- Swagger API documentation
- Rate limiting
- Refresh tokens

---

## License

This project is licensed under the MIT License.
