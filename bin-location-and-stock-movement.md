# Feature: Bin Location Tracking and Stock Movement Control

## Short Description
This feature assigns a specific physical location (bin, shelf, rack) to every item in the store and records every movement of stock in and out of that location.

## Purpose
To make it easy to locate items quickly in the warehouse, reduce time wasted searching for products, and maintain accurate records of stock movement for auditing.

## Main Functions / Activities
- Assigns bin location codes to items (e.g., Aisle A - Rack 2 - Shelf 3).
- Records Goods Received, Goods Issued, and Internal Stock Transfer.
- Implements FIFO (First In First Out) to prevent expiry of old stock.
- Shows real-time quantity per location.
- Generates low-stock and misplaced-stock alerts.
