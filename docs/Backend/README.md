---
layout: default
title: Backend API
nav_order: 4
has_children: true
permalink: /Backend/
---

# Backend API Documentation

Documentation for the Python-based backend services for the Personalized Travel Planning System.

## Technology Stack
- **Framework**: Flask (Python 3.x)
- **Database**: MySQL (Community Edition)
- **Middleware**: Flask-CORS for cross-origin resource sharing.

## Database Schema
The backend manages a database named `personalisedtravel` with the following key tables:
- **`user`**: Stores user authentication and profile data.
- **`Admin`**: Stores administrative credentials.
- **`destination`**: Lists all 14 districts in Kerala.
- **`hotel`**: Stores specific properties and their associated districts.
- **`room`**: Manages room types, pricing, and availability.
- **`facility`**: Stores optional amenities and their costs.
- **`payment`**: Records booking transactions and their status.

---

## 📂 Backend Files
- `server.py`
- `check_db.py`
- `force_seed.py`
