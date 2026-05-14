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

## 🏢 About Company (Nimap Infotech)

We help candidates start their IT career with:

* 50% year-on-year growth opportunities
* Real-time project exposure
* Strong technical mentorship
* Immediate project allocation via **NTTS (Nimap Talent Transformation System)**

---

## 👨‍💻 Author

Sandip Bhande
Pune, Maharashtra

```

---

## 📌 How to add this on GitHub

1. Open your repo on GitHub  
2. Click **Add file → Create new file**  
3. File name:
```

README.md

```
4. Paste this content  
5. Click **Commit new file**

---

If you want next step, I can also help you:
✔ Fix your GitHub push error (Repository not found)  
✔ Create full Docker + FastAPI code  
✔ Help you complete machine test perfectly for HR  

Just tell me 👍
```
