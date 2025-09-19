# Fullstack Docker App

A full-stack web application built with **React (frontend)**, **Express (backend)**, and **PostgreSQL (database)**.
This project demonstrates a simple architecture for connecting a React app to an Express API, which in turn communicates with a PostgreSQL database.


---

## 📂 Project Structure

fullstack-docker-app/
├── backend/
│ ├── app.js
│ └── package.json
├── frontend/
│ ├── package.json
│ └── src/
│ └── App.js
├── db-data/ --------------- --------------------- # For database volume
├── docker-compose.yml ----------------- # Empty,
├── .env -------------------------------------------- # Empty for future use.
└── README.md ------------------------------


---

## 🚀 Features

### ✅ Backend (Node.js + Express + PostgreSQL)
- Connects to PostgreSQL using `pg` library.
- Provides `/api` endpoint that returns the current server time from the database.
- Simple error handling for database connection issues.

### ✅ Frontend (React)
- Fetches API response from the backend.
- Displays the message in a minimal UI.
- Uses `"proxy": "http://localhost:5000"` to forward requests to the backend during development.

### ✅ Database (PostgreSQL)
- Managed through a Docker volume (`db-data/`).
- Configurable via environment variables in `.env` file.



