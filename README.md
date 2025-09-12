# 📋 task manager app!!

This is full-stack task management application that allows users to create, complete, and delete tasks in a clean and responsive UI. It uses **React** for the frontend, **Node.js + Express** for the backend, and **MongoDB** for data persistence.

---

## ✨ Features

- Create and manage tasks
- Toggle task completion status
- Delete tasks
- Store data in a MongoDB database
- Fully RESTful API
- Responsive frontend built with React

---

## 🗂 Project Structure

```
taskvault/
├── client/                # React frontend
│   ├── public/
│   ├── src/
│   │   ├── components/    # UI components (TaskForm, TaskList, etc.)
│   │   ├── App.js         # Main App
│   │   └── App.css        # Styling
├── server/                # Express backend
│   ├── models/            # Mongoose model for tasks
│   ├── routes/            # REST API routes
│   ├── server.js          # App entrypoint
│   └── .env               # Environment variables (MONGO_URI)
```

---

## 🚀 Getting Started

### 📌 Prerequisites

- Node.js and npm installed
- MongoDB Atlas or local MongoDB server

---

### 🧪 Backend Setup

```bash
cd server
npm install
```

1. Create a `.env` file in `/server` with:
   ```
   MONGO_URI=your_mongodb_connection_string
   ```

2. Start the server:

```bash
node server.js
```

> Runs on [http://localhost:5000](http://localhost:5000)

---

### 🌐 Frontend Setup

```bash
cd client
npm install
npm start
```

> Runs on [http://localhost:3000](http://localhost:3000)

---

## 🧠 API Endpoints

### `GET /api/tasks`
Returns all tasks (sorted by creation date).

### `POST /api/tasks`
Creates a new task.  
Body:
```json
{
  "title": "Read 10 pages"
}
```

### `PUT /api/tasks/:id`
