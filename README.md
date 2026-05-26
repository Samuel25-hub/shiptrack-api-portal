# ShipTrack API Documentation

Developer-focused REST API documentation portal built using Markdown, GitHub, and GitHub Pages.

This project demonstrates API documentation structure, authentication workflows, endpoint references, JSON request/response formatting, and developer onboarding documentation.

---

## Quick Links

- [Authentication](authentication.md)
- [Getting Started](getting-started.md)
- [Error Handling](errors.md)

### Endpoints
- [GET /shipments](endpoints/get-shipments.md)
- [POST /shipments](endpoints/create-shipment.md)
- [PUT /shipments/{id}](endpoints/update-shipment.md)

---

## Overview

ShipTrack API allows logistics companies to manage shipments, update delivery statuses, and retrieve shipment information through REST API endpoints.


## API Workflow Diagram

```text
Client Application
        │
        ▼
ShipTrack API Endpoint
        │
        ▼
Authentication Validation
        │
        ▼
Shipment Database
        │
        ▼
JSON Response Returned
```
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
| GET | [/shipments](endpoints/get-shipments.md) | Retrieve all shipments |
| POST | [/shipments](endpoints/create-shipment.md) | Create shipment |
| PUT | [/shipments/{id}](endpoints/update-shipment.md) | Update shipment |

---

## Response Format

All responses are returned in JSON format.
