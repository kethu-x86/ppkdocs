---
layout: default
title: HotelPage.jsx
parent: Frontend Source
nav_order: 22
---

# HotelPage.jsx

The hotel discovery and recommendation component.

## Purpose
Presents a curated list of hotels in the chosen district, specifically recommended based on the user's selected activities and budget.

## Key Features
- **Activity-Based Recommendations**: Groups hotels by their proximity to the user's chosen activities.
- **Budget Awareness**: Highlights "Best Match" hotels that fit within the user's set budget and flags "Premium" options.
- **Real-Time Availability**: Checks `localStorage` for any hotels disabled by the admin and reflects their "Fully Booked" status.
- **Commute Estimation**: Provides calculated travel distance and time (car/bike) from hotels to key activities.
- **Dynamic Hotel Data**: Contains a massive registry of hotels across all Kerala districts with ratings, images, and base prices.
- **AI Suggestions**: Automatically fills empty activity groups with suggested hotels in the same district.
- **Budget Alerts**: Displays a modal if no hotels in the district fit the user's budget and stay duration.
- **Silent Registration**: Ensures the hotel is registered in the database before proceeding to room selection.

## Data Structure
Extensive `districtHotels` and `hotelDistances` objects mapped by district and hotel IDs.
