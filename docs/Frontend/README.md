---
layout: default
title: Frontend Source
nav_order: 2
has_children: true
permalink: /Frontend/
---

# Frontend Source Code Documentation

This section provides a detailed breakdown of every file in the `src` directory of the Personalized Travel Planning System. The documentation follows the structure of the source tree.

## Architecture Overview

The application is built using **React 19**, **Vite**, and **Material UI**. It uses **React Router** for navigation and **Session Storage / Local Storage** for client-side state persistence.

### Key Functional Flows:
1. **User Auth:** Handled in `Login.jsx` (User) and `AdminLogin.jsx` (Admin).
2. **Trip Planning:** Initiated in `Login.jsx` with destination, budget, and date selection.
3. **Activity Discovery:** `DistrictPage.jsx` presents activities specific to the chosen Kerala district.
4. **Accommodation:** `HotelPage.jsx` and `RoomPage.jsx` handle hotel and room selection with budget-awareness.
5. **Booking:** `BookingPage.jsx` allows adding amenities and tracks the final grand total.
6. **Payment & History:** `PaymentPage.jsx` simulates processing and `HistoryPage.jsx` displays previous trips.

---

## 📂 Source Files
Listed below in their tree order.
