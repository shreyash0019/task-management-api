
# Task Management API

## 📌 Overview

This is a simple RESTful API built with **Node.js** and **Express** that allows users to perform basic **CRUD operations** on tasks (to-do items). It uses **in-memory storage** (no database), with support for **Swagger UI documentation**.

---

## 🚀 Features

- Create, Read, Update, and Delete tasks
- Input validation
- In-memory storage
- RESTful routing
- Error handling
- Swagger-based API documentation
- Sample data on startup

---

## 🔧 Installation & Running

1. **Clone the repo**
```bash
git clone https://github.com/shreyash0019/task-management-api.git
cd task-management-api
```

2. **Install dependencies**
```bash
npm install
```

3. **Start the server**
```bash
node index.js
```

4. Visit `http://localhost:3000/api-docs` for Swagger API documentation

---

## 📂 Endpoints

### ✅ `GET /tasks`

- **Description**: Get all tasks
- **Response**:
```json
[
  {
    "id": 1,
    "title": "Design homepage",
    "description": "Create wireframes for the homepage"
  }
]
```

---

### ✅ `GET /tasks/:id`

- **Description**: Get a task by its ID
- **Response**:
```json
{
  "id": 1,
  "title": "Design homepage",
  "description": "Create wireframes for the homepage"
}
```

---

### ✅ `POST /tasks`

- **Description**: Create a new task
- **Request Body**:
```json
{
  "title": "Create login page",
  "description": "Design and implement the login page"
}
```

- **Response**:
```json
{
  "id": 3,
  "title": "Create login page",
  "description": "Design and implement the login page"
}
```

---

### ✅ `PUT /tasks/:id`

- **Description**: Update an existing task
- **Request Body**:
```json
{
  "title": "Updated Task Title",
  "description": "Updated Task Description"
}
```

---

### ✅ `DELETE /tasks/:id`

- **Description**: Delete a task by ID
- **Response**:
```json
{
  "message": "Task deleted successfully"
}
```

---

## 📘 API Documentation (Swagger)

- **URL**: [http://localhost:3000/api-docs](http://localhost:3000/api-docs)
- Auto-generated using `swagger-jsdoc` and `swagger-ui-express`

---

## 💡 Sample Tasks on Startup

```json
[
  {
    "id": 1,
    "title": "Design homepage",
    "description": "Create wireframes for the homepage"
  },
  {
    "id": 2,
    "title": "API integration",
    "description": "Connect frontend with backend REST API"
  }
]
```

---
