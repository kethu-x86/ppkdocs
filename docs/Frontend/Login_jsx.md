---
layout: default
title: Login.jsx
parent: Frontend Source
nav_order: 24
---

# Login.jsx

The user authentication and primary trip planner component.

## Purpose
Acts as the central gateway for users to log in, register, and initiate their travel package design.

## Key Features
- **Dual Functionality**: Handles both login and registration via a toggled interface.
- **Backend Authentication**: Connects to `http://127.0.0.1:5000/login` and `http://127.0.0.1:5000/register`.
- **Primary Trip Planner**: A comprehensive form for logged-in users to set their destination, budget, dates, and number of travelers.
- **Global Search**: Features a header-based search input to quickly find specific hotels or destinations.
- **District Discovery**: Contains a visual registry of all Kerala districts with imagery to help users choose.
- **Admin Access Link**: A dedicated button to navigate to the `AdminLogin` page.
- **Planner Validation**: Ensures all required fields are filled before initiating the trip selection flow.

## State Management
- `isLoggedIn`: Tracks authentication status via `sessionStorage`.
- `selectedDest`, `budget`, `startDate`, etc.: Captures trip planning parameters.
