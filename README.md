Here is a **GitHub-ready README.md** you can directly paste into your repository (clean, professional, and submission-ready):

---

```md
# Docker FastAPI Test Project

This project is a simple FastAPI application containerized using Docker and Docker Compose.  
It demonstrates REST APIs with file-based storage (no database used).

---

## 🚀 Features

- FastAPI backend
- Docker containerization
- Docker Compose setup
- File-based storage using `users.json`
- Persistent data even after container restart
- Swagger UI for API testing

---

## 📂 Project Structure

```

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

## 📌 API Endpoints

### Home

```

GET /

````

Response:
```json
{
  "message": "Hello World"
}
````

---

### Get All Users

```
GET /users
```

Returns list of users stored in `users.json`.

---

### Add User

```
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

## 🐳 Run Project with Docker

### Step 1: Build and Run

```bash
docker-compose up --build
```

### Step 2: Stop Containers

```bash
docker-compose down
```

---

## 🔁 Data Persistence Test

1. Run container
2. Add users using `/users` API
3. Stop container
4. Start again

👉 Data will still be available in `data/users.json`

---

## 📖 API Documentation (Swagger)

After running the project, open:

```
http://localhost:8000/docs
```

---

## 🛠 Tech Stack

* Python
* FastAPI
* Docker
* Docker Compose

---


