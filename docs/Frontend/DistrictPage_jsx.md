---
layout: default
title: DistrictPage.jsx
parent: Frontend Source
nav_order: 18
---

# DistrictPage.jsx

The itinerary building and activity selection component.

## Purpose
Provides a district-specific overview of activities and landmarks for users to add to their travel package.

## Key Features
- **Dynamic Content**: Displays a curated list of activities for each Kerala district (Kasaragod, Kannur, etc.).
- **Interactive Map/Grid**: A visually rich grid of activity cards with icons and descriptions.
- **Activity Discovery**: Detailed info sections for each activity to help users make informed choices.
- **Itinerary Persistence**: Saves selected activities to the backend via `http://127.0.0.1:5000/saveTrip`.
- **Search Context**: Maintains the budget and date context from the main planner throughout the selection process.
- **Seamless Transition**: Navigates to the `HotelPage` with all activity selections passed as URL parameters.

## Data Structure
Contains a comprehensive data object mapped by district name, including activity IDs, names, icons, and descriptions.
