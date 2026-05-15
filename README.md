# Docker FastAPI Test Project

A simple and lightweight FastAPI application containerized using Docker and Docker Compose.  
This project demonstrates REST API development with file-based storage using `users.json` instead of a database.

---

## Features

- FastAPI backend
- RESTful API endpoints
- Docker containerization
- Docker Compose configuration
- File-based storage using `users.json`
- Persistent data after container restart
- Interactive Swagger UI documentation
- Beginner-friendly project structure

---

## Project Structure

```text
.
├── app
│   ├── main.py
│   ├── routes.py
│   ├── models.py
│   └── data
│       └── users.json
├── Dockerfile
├── docker-compose.yml
├── requirements.txt
└── README.md
```

---

## Requirements

Before running the project, install:

- Docker
- Docker Compose

---

## Getting Started

### Clone the Repository

```bash
git clone https://github.com/sandipbhande/docker-fastapi-test.git
cd docker-fastapi-test
```

---

### Build and Run the Application

```bash
docker-compose up --build
```

Application will run at:

```text
http://localhost:8000
```

---

## 📚 API Documentation

### Swagger UI

```text
http://localhost:8000/docs
```

### ReDoc

```text
http://localhost:8000/redoc
```

---

## 🔗 API Endpoints

### Home Endpoint

```http
GET /
```

#### Response

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

Returns all users stored in `users.json`.

---

### Add User

```http
POST /users
```

#### Request Body

```json
{
  "id": 1,
  "name": "John Doe",
  "email": "john@example.com"
}
```

#### Response

```json
{
  "message": "User added successfully"
}
```

---

## Data Persistence

User data is stored in:

```text
app/data/users.json
```

Data remains available even after restarting the container.

---

## Docker Commands

### Start Containers

```bash
docker-compose up
```

### Build and Start Containers

```bash
docker-compose up --build
```

### Stop Containers

```bash
docker-compose down
```

### Check Running Containers

```bash
docker ps
```

---




##  License

This project is for learning and assessment purposes.


