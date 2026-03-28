---
layout: default
title: check_db.py
parent: Backend API
nav_order: 2
---

# check_db.py

A database verification utility.

## Purpose
A command-line script for developers to quickly check the current status and integrity of the MySQL database.

## Key Features
- **Connectivity Test**: Verifies a successful connection to the `personalisedtravel` database.
- **Statistics Report**: Prints the total count of destinations and hotels currently registered.
- **Search Verification**: Performs a series of test queries (e.g., searching for "Halifax" or "Kasaragod") to ensure the search logic is functioning correctly.
- **Join Verification**: Tests complex `JOIN` queries between the `hotel` and `destination` tables to confirm foreign key relationships.
