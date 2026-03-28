---
layout: default
title: FacilitiesPage.jsx
parent: Frontend Source
nav_order: 19
---

# FacilitiesPage.jsx

The room-specific facility customization component.

## Purpose
A focused view for selecting and reviewing amenities for a specific room type before finalizing the booking.

## Key Features
- **Selection Persistence**: Allows users to toggle standard and premium facilities (WiFi, AC, TV, etc.).
- **Live Pricing**: Dynamically calculates the total cost of all selected facilities.
- **Contextual View**: Shows current hotel and room type for a personalized experience.
- **Confirm & Return**: Provides a clear confirmation path to return to the previous booking step.
- **Visual Feedback**: Real-time styling updates to highlight selected items.

## Key State
- `selected`: Array of facility IDs chosen by the user.
- `defaultFacilities`: Registry of all possible amenities with names, icons, and prices.
