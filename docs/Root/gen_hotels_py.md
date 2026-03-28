---
layout: default
title: gen_hotels.py
parent: Root Files
nav_order: 6
---

# gen_hotels.py

Automation script for hotel data generation.

## Purpose
A Python utility script used to programmatically generate and inject hotel data into the `HotelPage.jsx` and `AdminDashboard.jsx` files.

## Key Functions
- **Data Mapping**: Defines a structure for districts and their associated activities.
- **Randomized Assignments**: Randomly assigns hotels, prices, ratings, and tags to various districts.
- **File Injection**: Uses regular expressions (`re`) to find the `districtHotels` and `allHotels` arrays in the source code and update them with fresh data.
- **Asset Integration**: Links Unsplash-based imagery to each generated hotel.

## Key Logic
- Groups 6 hotels per district with varying tiers (Luxury, Budget, Homestay, etc.).
- Calculates simulated commute distances to activity sites for each hotel.
