---
layout: default
title: SearchResults.jsx
parent: Frontend Source
nav_order: 28
---

# SearchResults.jsx

The global search discovery and trip-starting component.

## Purpose
Displays all matching destinations and hotels for a user's search query, allowing them to initiate a custom trip plan directly from search.

## Key Features
- **Global API Integration**: Fetches unified results from `http://127.0.0.1:5000/search?q=...`.
- **Destination Discovery**: Allows users to select a district from search, which triggers a trip-planning modal (dates, budget, etc.) to start the flow.
- **Hotel Deep-Dive**: Users can click any hotel to view available room types and prices in a dynamic dropdown.
- **Room API Integration**: Fetches real-time room availability for a specific HID via `http://127.0.0.1:5000/hotel/HID/rooms`.
- **Direct Booking Path**: Provides a "Book Now" shortcut from search directly to the booking summary.
- **Modal Logic**: Centrally manages the trip-planner modal used to gather itinerary details for new destinations.

## Key State
- `results`: Object containing separate arrays for `destinations` and `hotels`.
- `loading`: Tracks the status of the primary search query.
- `selectedHotel`: Manages the state of the active hotel dropdown.
- `isModalOpen`: Controls the visibility of the destination-to-trip-plan transition modal.
