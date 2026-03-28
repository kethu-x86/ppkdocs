---
layout: default
title: App.jsx
parent: Frontend Source
nav_order: 2
---

# App.jsx

The main application component and routing hub.

## Purpose
Defines the application's layout and client-side routing using `react-router-dom`.

## Routes Defined
- **`/`**: The main login and trip planning page (`Login.jsx`).
- **`/district/:name`**: District activities selection (`Districtpage.jsx`).
- **`/search-results`**: Search functionality for destinations and hotels (`SearchResults.jsx`).
- **`/hotels` & `/hotels/:name`**: Hotel search results for a chosen district (`HotelPage.jsx`).
- **`/rooms/:districtName/:hotelName`**: Room selection for a specific hotel (`RoomPage.jsx`).
- **`/facilities/:hotelName/:roomType`**: Additional amenity customization (`FacilitiesPage.jsx`).
- **`/booking/:hotelName/:roomType`**: Final booking summary and selection (`BookingPage.jsx`).
- **`/payment`**: Secure payment simulation (`PaymentPage.jsx`).
- **`/history`**: Personal travel history (`HistoryPage.jsx`).
- **`/admin-login`**: Administrative access entry (`AdminLogin.jsx`).
- **`/admin-dashboard`**: Admin-only control panel for hotel management (`AdminDashboard.jsx`).

## Key Dependencies
- `react-router-dom`: Handles all navigation within the SPA.
