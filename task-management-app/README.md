# TaskFlow — Task Management Application

Full-stack task manager built with React, Vite, Node.js, Express and MongoDB.

## Features
- User registration and login with JWT authentication
- Create, read, update and delete tasks
- Task status, priority and due date
- Search and status filters
- Responsive desktop/mobile UI
- Protected task API routes

## 1. Backend setup
```bash
cd backend
npm install
copy .env.example .env
```
Edit `.env` and add your MongoDB connection string and JWT secret.

Run:
```bash
npm run dev
```
Backend: `http://localhost:5000`

## 2. Frontend setup
Open a second terminal:
```bash
cd frontend
npm install
copy .env.example .env
npm run dev
```
Open the Vite URL shown in the terminal, normally `http://localhost:5173`.

## MongoDB
Create a MongoDB Atlas database, allow your development IP in Network Access, create a database user, and copy the connection string into `backend/.env` as `MONGO_URI`.

## Deployment
Deploy `backend` as a Node service and `frontend` as a static/Vite site. Set:
- Backend: `MONGO_URI`, `JWT_SECRET`, `PORT`
- Frontend: `VITE_API_URL=https://YOUR-BACKEND-URL/api`

Do not commit `.env` files or passwords.
