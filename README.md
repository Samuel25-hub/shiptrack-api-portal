# ShipTrack API Documentation

## Overview

ShipTrack API allows logistics companies to manage shipments, update delivery statuses, and retrieve shipment information through REST API endpoints.

---

## Base URL

```text
https://api.shiptrack.com/v1
```

---

## Authentication

All API requests require Bearer Token authentication.

### Example

```text
Authorization: Bearer YOUR_API_KEY
```

---

## Available Endpoints

| Method | Endpoint | Description |
|---|---|---|
| GET | /shipments | Retrieve all shipments |
| GET | /shipments/{id} | Retrieve shipment details |
| POST | /shipments | Create shipment |
| PUT | /shipments/{id} | Update shipment |

---

## Response Format

All responses are returned in JSON format.
