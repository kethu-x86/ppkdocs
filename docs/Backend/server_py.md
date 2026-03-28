---
layout: default
title: server.py
parent: Backend API
nav_order: 1
---

# server.py

The core backend API server.

## Purpose
A Flask-based application that handles all API requests from the React frontend, manages database interactions, and ensures the schema is correctly initialized.

## Key API Endpoints
- **`/register` & `/login`**: User authentication services.
- **`/adminLogin`**: Secure access for administrative users.
- **`/saveTrip`**: Records selected activities for a specific district.
- **`/bookHotel`**: Silently registers a hotel into the database before room selection.
- **`/reserveRoom`**: Saves a specific room reservation and generates a unique RID (Room ID).
- **`/saveFacilities`**: Records all paid amenities selected by the user.
- **`/savePayment`**: Finalizes the booking process by recording the payment status and amount.
- **`/search`**: A global, case-insensitive search engine for destinations and hotels.
- **`/hotel/<hid>/rooms`**: Retrieves all available room types for a specific hotel.

## Core Features
- **Database Auto-Initialization**: Automatically creates the `personalisedtravel` database and all required tables if they do not exist.
- **CORS Handling**: Configures Cross-Origin Resource Sharing to allow communication with the Vite frontend.
- **Error Logging**: Provides detailed server-side logs for database connection issues and API failures.
