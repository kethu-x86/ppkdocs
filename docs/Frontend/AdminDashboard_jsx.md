---
layout: default
title: AdminDashboard.jsx
parent: Frontend Source
nav_order: 15
---

# AdminDashboard.jsx

The administrative control panel component.

## Purpose
Provides a central interface for administrators to manage the global hotel inventory, including enabling or disabling specific stays for booking.

## Key Features
- **Access Control**: Verifies `sessionStorage` for administrative privileges before allowing access.
- **Inventory Management**: Displays a comprehensive list of all hotels across various districts in Kerala.
- **District Filtering**: Allows admins to quickly narrow down the list of hotels by their respective districts.
- **Status Toggling**: Real-time control to enable or disable hotels (e.g., for maintenance or fully-booked status), with state persisted in `localStorage`.
- **Administrative Logout**: Safely clears session data and redirects to the admin login.

## Data Structure
Contains a hardcoded registry of all hotels with unique HIDs (Hotel IDs).
