---
layout: default
title: Setup & Installation
nav_order: 5
permalink: /SETUP/
---

# Setup & Installation Guide

Follow these steps to get the Personalized Travel Planning System running on your local machine.

## Prerequisites
- **Node.js** (v18 or higher)
- **Python** (v3.10 or higher)
- **MySQL** (Community Edition)
- **npm** or **yarn**

---

## 🖥️ Frontend Setup (React)

1. **Navigate to the root directory**:
   ```bash
   cd project
   ```
2. **Install dependencies**:
   ```bash
   npm install
   ```
3. **Start the development server**:
   ```bash
   npm run dev
   ```
   The application should now be running at `http://localhost:5173`.

---

## ⚙️ Backend Setup (Flask)

1. **Navigate to the backend directory**:
   ```bash
   cd backend
   ```
2. **Install Python dependencies**:
   ```bash
   pip install flask flask-cors mysql-connector-python
   ```
3. **Configure MySQL**:
   - Ensure MySQL is running on `localhost`.
   - Update the `config` object in `server.py` with your MySQL `user` and `password`.
4. **Seed the database**:
   ```bash
   python force_seed.py
   ```
5. **Start the server**:
   ```bash
   python server.py
   ```
   The backend API will be available at `http://127.0.0.1:5000`.

---

## 🗄️ Database Management

- **Verify Data**: Run `python check_db.py` to ensure all destinations and hotels are correctly loaded.
- **Refresh Stays**: Use `python ../gen_hotels.py` from the root to refresh the hotel registry in the source code.
