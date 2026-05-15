# Docker FastAPI Test Project

A simple FastAPI application containerized using Docker and Docker Compose.
The project demonstrates REST APIs with file-based storage using `users.json` without a database.

---

## Features

* FastAPI backend
* Docker containerization
* Docker Compose setup
* File-based storage using `users.json`
* Persistent data after container restart
* Swagger UI for API testing

---

## Project Structure

```text
.
├── app
│   ├── main.py
│   ├── routes.py
│   ├── models.py
│   └── data/
│       └── users.json
├── Dockerfile
├── docker-compose.yml
├── requirements.txt
└── README.md
```

---

## API Endpoints

### Home

```http
GET /
```

Response:

```json
{
  "message": "Hello World"
}
```

---

### Get All Users

```http
GET /users
```

Returns the list of users stored in `users.json`.

---

### Add User

```http
POST /users
```

Request Body:

```json
{
  "id": 1,
  "name": "John",
  "email": "john@example.com"
}
```

Response:

```json
{
  "message": "User added successfully"
}
```

---

## Run the Project

### Build and Start Containers

```bash
docker-compose up --build
```

### Stop Containers

```bash
docker-compose down
```

---

## Data Persistence

1. Start the container
2. Add users using the `/users` API
3. Stop the container
4. Start the container again

The data will remain available in `data/users.json`.

---



