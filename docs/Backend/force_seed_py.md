---
layout: default
title: force_seed.py
parent: Backend API
nav_order: 3
---

# force_seed.py

A database refresh and seeding utility.

## Purpose
A critical tool for resetting the application's core data by dropping existing tables and re-populating them with a fresh, comprehensive set of data.

## Key Actions
- **Schema Refresh**: Disables foreign key checks, drops `hotel` and `destination` tables, and recreates them from scratch.
- **Seeding destinations**: Populates the `destination` table with all 14 official Kerala districts and an "Other" category.
- **Seeding hotels**: Injects over 100 unique hotels across the various districts, providing a diverse set of options for testing and development.
- **Foreign Key Enforcement**: Safely re-enables foreign key checks after the data has been successfully seeded.

## Usage
Should be run during the initial setup or when a clean data state is required for development or testing.
