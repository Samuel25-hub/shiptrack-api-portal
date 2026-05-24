# Getting Started

This guide shows you how to make your first request to the ShipTrack API.

---

## Step 1: Get an API Key

To use the ShipTrack API, you need an API key from your developer dashboard.

Example:

```text
YOUR_API_KEY
```

---

## Step 2: Add Authorization Header

Include your API key in the request header.

```text
Authorization: Bearer YOUR_API_KEY
```

---

## Step 3: Make Your First Request

Use the following cURL command to retrieve shipments:

```bash
curl -X GET https://api.shiptrack.com/v1/shipments \
-H "Authorization: Bearer YOUR_API_KEY"
```

---

## Step 4: Review the Response

Example response:

```json
{
  "shipments": [
    {
      "shipment_id": "ST-1001",
      "status": "In Transit",
      "destination": "Houston, TX"
    }
  ]
}
```

---

## Next Steps

After making your first request, review the available endpoint documentation:

- [GET /shipments](endpoints/get-shipments.md)
- [POST /shipments](endpoints/create-shipment.md)
