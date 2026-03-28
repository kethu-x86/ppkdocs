---
layout: default
title: AdminLogin.jsx
parent: Frontend Source
nav_order: 16
---

# AdminLogin.jsx

The administrative authentication component.

## Purpose
Provides a secure login form specifically for system administrators to access the dashboard.

## Key Features
- **API Integration**: Connects to the `http://127.0.0.1:5000/adminLogin` endpoint for verification.
- **Form Validation**: Standard required-field validation for admin username and password.
- **Session Management**: Upon successful login, sets `isAdmin` and `userName` in `sessionStorage`.
- **Error Handling**: Gracefully handles backend connection issues and invalid credential alerts.
- **Secure Navigation**: Redirects to the `AdminDashboard` only after successful authentication.
