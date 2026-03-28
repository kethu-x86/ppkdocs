---
layout: default
title: PaymentPage.jsx
parent: Frontend Source
nav_order: 25
---

# PaymentPage.jsx

The secure payment simulation and booking finalization component.

## Purpose
Simulates a secure credit card payment process and records the final booking data to both the database and local history.

## Key Features
- **Payment Processing**: Mock processing with a delay for realism, using `http://127.0.0.1:5000/savePayment`.
- **Form Data Capture**: Collects card name, number, expiry, and CVV with basic validation and mask styling.
- **Booking History**: Automatically saves a detailed booking object to `localStorage`'s `bookingHistory` array on success.
- **Success Confirmation**: Provides a dedicated success view with green-themed branding and links to Home or History.
- **Dynamic Pricing**: Shows the total amount to be paid based on all previous selections (rooms, facilities, etc.).
- **Data Robustness**: Uses URL parameters and fallback `sessionStorage` (current HID) to ensure booking context is maintained.
- **Security Trust Signals**: Displays SSL encryption badges and secure footer messaging.

## Key State
- `isProcessing`: Tracks simulated network request state.
- `isSuccess`: Toggles between the payment form and the confirmation view.
