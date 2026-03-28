---
layout: default
title: RoomPage.jsx
parent: Frontend Source
nav_order: 26
---

# RoomPage.jsx

The room selection and detailed property exploration component.

## Purpose
Displays specific room types, descriptions, and ratings for a chosen hotel, while also providing info on nearby amenities.

## Key Features
- **Dynamic Room Inventory**: Generates themed room lists (Standard, Deluxe, Executive, etc.) based on the hotel's character if hardcoded data is not present.
- **Budget Filtering**: Only displays room types where the total stay cost (for the required number of rooms and nights) is within the user's budget.
- **Quantity Selector**: Automatically calculates the minimum number of rooms needed based on the guest count (2 adults per room).
- **Nearby Exploration**: A comprehensive modal showcasing local petrol stations, EV chargers, food spots, and shopping centers based on the user's chosen activities.
- **Reservation Logic**: Silently ensures the hotel is in the database before saving the specific room reservation via `http://127.0.0.1:5000/reserveRoom`.
- **Budget Tracking**: Real-time cost updates and modals if users try to select more rooms than their budget allows.

## Key Functions
- `getDynamicRooms()`: Logic for diversifying the room options based on hotel name.
- `handleReserveRoom()`: Validates and initiates the room booking process.
