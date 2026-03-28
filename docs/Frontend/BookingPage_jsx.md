---
layout: default
title: BookingPage.jsx
parent: Frontend Source
nav_order: 17
---

# BookingPage.jsx

The final package customization and booking summary component.

## Purpose
Allows users to add extra amenities and review their personalized travel package before final payment.

## Key Features
- **Amenity Customization**: Provides a list of facilities (WiFi, AC, Breakfast, etc.) with real-time price updates.
- **Budget Tracking**: Dynamically updates a progress bar to show how the current total compares to the user's set budget.
- **Budget Alerts**: Triggers a modal warning if adding a specific facility would exceed the allocated budget.
- **Data Persistence**: Saves selected facilities to the backend via `http://127.0.0.1:5000/saveFacilities`.
- **Package Summary**: Calculates the grand total including room price, facility charges, and service fees.
- **Secure Handoff**: Passes all trip details to the `PaymentPage` via URL parameters for final processing.

## State Management
Uses `useState` to track selected facilities and `useMemo` for cost calculations.
