# GET /shipments

Retrieve all shipments associated with your account.

---

## Endpoint

```text
GET /shipments
```

---

## Example Request

```bash
curl -X GET https://api.shiptrack.com/v1/shipments \
-H "Authorization: Bearer YOUR_API_KEY"
```

---

## Example Response

```json
{
  "shipments": [
    {
      "shipment_id": "ST-1001",
      "status": "In Transit",
      "destination": "Houston, TX"
    },
    {
      "shipment_id": "ST-1002",
      "status": "Delivered",
      "destination": "Dallas, TX"
    }
  ]
}
```

---

## Status Codes

| Code | Meaning |
|---|---|
| 200 | Success |
| 401 | Unauthorized |
| 500 | Internal Server Error |
