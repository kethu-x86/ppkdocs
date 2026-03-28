---
layout: default
title: HistoryPage.jsx
parent: Frontend Source
nav_order: 21
---

# HistoryPage.jsx

The user's travel history and booking record component.

## Purpose
Displays a comprehensive list of all past and upcoming bookings made by the currently logged-in user.

## Key Features
- **User-Specific Filtering**: Automatically filters the global `localStorage` history to only show records for the active `userName`.
- **Comprehensive Details**: Shows each booking's hotel, room type, travelers, dates, and total amount.
- **Activity & Facility Tags**: Visualizes chosen activities and facilities as a tag cloud for quick recall.
- **Confirmed Status**: Displays a clear "Confirmed" badge for all completed reservations.
- **Empty State**: Provides a helpful "Plan a Trip Now" call-to-action if no history is found.
- **Data Source**: Synchronizes with `localStorage` to persist travel records across sessions.

## Key State
- `history`: Local array of booking objects for the current user.
